#Distributed Tensorflow :

First, lets see a simple example of running multiple tasks using distributed tensor flow.
```python
# test.py
jobName = sys.argv[1]
taskIndex = sys.argv[2]
worker = ['localhost:2221', 'localhost:2222']
cluster = tf.train.ClusterSpec({"worker": worker})
# Create and start a server for the local task.
server = tf.train.Server(cluster, job_name=jobName, task_index=taskIndex)
if jobName == 'worker':
	W = tf.Variable(1, trainable=False, dtype=tf.int32, name='W')
	init_op = tf.global_variables_initializer()
	with tf.Session() as sess:
	sess.run(init_op)
	for i in range(10):
		incr = tf.assign(W, W + 1)
		print sess.run(incr)
		time.sleep(3)
```
```sh
python test.py worker 0
python test.py worker 1
```