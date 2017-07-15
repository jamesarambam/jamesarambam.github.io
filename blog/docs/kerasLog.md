#Keras with Log Likelihood Loss :

	"""
	++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
	Author : James Arambam
	Date   : 15 Jul 2017
	Description :
	Input : 
	Output : 
	++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
	"""

	from keras.models import Sequential
	from keras.layers import Dense
	import tensorflow as tf

	def logLike_Loss(y_true, y_pred):
    	return tf.log(y_pred)

    x_train = [[1, 2, 3, 4],
               [5, 6, 7, 8],
               [9, 10, 11, 12]
               ]
    y_train = [[],[], []]
    x_test = [[1, 2, 3, 4]]
    model = Sequential()
    model.add(Dense(3, activation='relu', input_dim=4))
    model.add(Dense(2, activation='softmax'))
    x = tf.placeholder(tf.float32, shape=(None, 4))
    model.compile(loss=logLike_Loss, optimizer='adam')
    model.fit(x_train, y_train, nb_epoch=10)
    y = model(x)
    with tf.Session() as sess:
        tf.initialize_all_variables().run()
        print sess.run(y, feed_dict={x : x_test})

