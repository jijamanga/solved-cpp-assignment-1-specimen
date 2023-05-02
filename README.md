Download Link: https://assignmentchef.com/product/solved-cpp-assignment-1-specimen
<br>
Introduction

<ul>

 <li>You have an HSI camera that is giving you 16-bit 2D images of width and height.</li>

 <li>Let’s assume that you are using an imaginary SDK which is giving you the images.</li>

 <li>Let’s assume that you have already registered a callback function (see below) for retrieving images from the camera’s SDK.</li>

</ul>

Callback Syntax

void onDataCallback(unsigned short* dataPtr, int width, int height)

{

// This function will be automatically called by an imaginary SDK (from its own thread).

}

<ul>

 <li>You can write this function to your example code and assume that it will get called automatically everytime a new image is incoming.</li>

 <li>The camera also has features that might change the image width and height on-the-fly. The new width and height will always be dividible by 2.</li>

 <li>If that happens; the updated width and height values will be given as parameters on the next time the callback function is called.</li>

</ul>




<table width="744">

 <tbody>

  <tr>

   <td width="744">Your Task: • Write a producer-consumer implementation for writing and reading images to/from memory buffers.•     Write a separate simple example code of using your implementation. This example code also contains the imaginary SDK and its callback function ‘onDataCallback’.</td>

  </tr>

 </tbody>

</table>




Notes:

<ul>

 <li>The implementation and the example doesn’t need to compile (so typos are ok), but other than that it should be valid C++ code.</li>

 <li>You can use libraries/frameworks if you want to. Just add the include and a comment on what library you are using.</li>

 <li>Consider that both the producer and the consumer might be used concurrently from different threads.</li>

 <li>The ‘onDataCallback’ function is called from another thread created by the SDK.</li>

 <li>The maximum width of the image is 640 and the maximum height of the image is 512. These values will not be surpassed.</li>

</ul>