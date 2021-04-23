# SpaceInvaders-RL
A Space Invader Bot.<br>
The Colab version will not show a display and should be used only for training, you can save the weights and load them on a local machine to see the run.<br>
Not all weights are in repository do to large size they can be found <a href="https://drive.google.com/drive/folders/1qkTTW8VVzlT7anssKVPnE-UuFqJv9fhI?usp=sharing">here</a>.
Only dqn.h5f.data-00000-of-00001 is not available in repository.<br>
The weights are for<br>
    model= Sequential()#sequential layer<br>
    model.add(Conv2D(32,(8,8),strides=(4,4), activation='relu', input_shape=(3, height, width,channels)))#32 no of filters 8 is filter size and 4 is stride width<br>
    model.add(Conv2D(64,(4,4), strides=(2,2), activation='relu'))<br>
    model.add(Flatten())<br>
    model.add(Dense(512,activation='relu'))<br>
    model.add(Dense(256,activation='relu'))<br>
    model.add(Dense(actions,activation='linear'))<br>
