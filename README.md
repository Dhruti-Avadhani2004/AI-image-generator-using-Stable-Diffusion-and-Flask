# AI-image-generator-using-Stable-Diffusion-and-Flask
Everything you need to build your very own version of an AI image generator using Stable Diffusion and Flask (Python)

<br>
<h3>Introduction</h3>
When curiosity meets fun, that's when things like this get built. There are a million ways that you can build an AI image generator, but in this project that I built, I had a few main problems that I wished to address; and still build this model successfully. This is probably my first ever project in the space of Gen-AI and I had so much to learn from it. Hoping to develop much better models in the future. 
<br>
<h3>How the Project Came to Life</h3>
Let us now look at the problems that I faced while developing this project and how I found a solution at each step. 
"Problem 1" :  AI model, that could help me generate images based on prompts
"addressing it" : Since this is my first attempt at a project like this, I thought of using a pretrained model so that I wouldn't have to undergo the hassle, from collecting and building data sets to training the model. Using a pretrained model made my job much easier. Initially, I thought of using Dall-E, by OpenAI, and after building about half the project using Tkinter, did I realise that I need to pay to make use of this model :(... Hence, I switched to using Stable Diffusion, which is practically, FREE!

"Problem 2" : Lack of GPU
"addressing it" : My computer is a simple student computer, nothing fancy. This machine, doesn't have a GPU. Hence, I needed to make use of any makeshift system that could provide me with GPU. And since I was comfortable with using Google Colab, I went ahead with the T4 GPU runtime in colab. 

"Problem 3" : Connecting my Flask Application to my Colab Notebook
"addressing it" : So, the idea of the project in my head was like this. The user would prompt the kind of image that needs to be generated using the Flask application as the frontend and the prompt gets processed in the colab notebook, and it generates an image (using colab notebook as the backend). The generated image would be sent back to the Flask application and displayed onto the screen. Now since the colab notebook and my Flask application were two different entities, I needed to find a way to connect them and make communication possible between them. I again chose a simpler and cheaper approach and went ahead with using an ngrok pipeline. It is a little hassle to get the pipeline up and running each time I want to use this application, but this is the best that could be done now. 

<br>
After a lot of trial and errors, I was finally able to make this application. You can find all the required resources and code, so that you too can build this project!
