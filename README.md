# ML App
# This app format helps to integrate the machine learning algorithms in android with the help of Tensorflow Lite.

An asset folder is created that contains the python code saved in .tf5 extension as app\src\main\assets. <br />
Then    implementation 'org.tensorflow:tensorflow-lite:+'   is implemented in app build.gradle. And an Interpreter <br />
is used as follows:- 
<pre>
  Interpreter interpreter;                                                                                                                                                                          
  try {  
            interpreter=new Interpreter(loadModelFile(),null);  
       }   <br />
       catch (IOException e)  {   
            e.printStackTrace();  
       }
</pre>
loadModelFile() can be found in MainActivity.java.        


