# ML App
This app format helps to integrate the machine learning algorithms in android with the help of Tensorflow Lite.

An asset folder is created that contains the python code saved in .tfs extension as app\src\main\assets.
Then {implementation 'org.tensorflow:tensorflow-lite:+'} is implemented in app build.gradle. And an Interpreter
is used as follows:-
  Interpreter interpreter;
  try {
            interpreter=new Interpreter(loadModelFile(),null);
       } 
       catch (IOException e)  {
            e.printStackTrace();
        }
loadModelFile() can be found in MainActivity.java.        


