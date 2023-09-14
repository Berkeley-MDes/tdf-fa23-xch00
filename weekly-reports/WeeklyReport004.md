# WeeklyReport004

## Clara(Xuechun) Zang💭20230907

---

![2.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/2.jpg)

Last week, I conducted a more in-depth analysis of the phone stand from a computational design perspective and contemplated using computational methods for topology optimization of the support structure.

![3.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/3.jpg)

For this project, I utilized the Grasshopper plugin Ameba, a specialized tool for conducting topology optimization using mechanics. Due to its reliance on cloud computing, it is highly lightweight. This optimization not only saved a significant amount of materials but also enhanced the structural aesthetics from a mechanical perspective.

![Untitled](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/Untitled.png)

First, I baked the model from the TJ video into Rhino. Then, I selected the BREP and imported it into Ameba as a battery block, converting it into a triangular mesh.

![5.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/5.jpg)

Below, I will introduce the specific steps for you.， Configure Ameba for topology optimization. This will involve defining constraints, objectives, and other optimization parameters to meet my design requirements.

![6.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/6.jpg)

Importing the selected geometry into Ameba. Create mesh file from closed brep

![7.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/7.jpg)

Then set constraints for the supporting surfaces and three-dimensional coordinates. Because I do not want any displacement in the structure, I have set them to 0.

![8.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/8.jpg)

The third step is to set shape constraints, and here I encountered many problems. I will explain them in detail next.

![9.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/9.jpg)

Afterward, set the optimization parameters and specify the number of iterations.

![10.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/10.jpg)

Next is setting the material for predicting stress, and I chose ABS.

![11.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/11.jpg)

After logging into the account, I began the cloud computing process. This was my first time trying cloud computing, and I have to admit I felt a bit nervous when I pressed the "start" button.

![12.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/12.jpg)

At this point, I set it for 109 iterations with 10,000 mesh faces to simulate. I also encountered some issues during the process.

![22222.jpg](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/22222.jpg)

The first time, I didn't set bottom constraints, which resulted in a loss of form.

![111111.jpg](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/111111.jpg)

After adding bottom constraints, I realized that the top constraints were not properly set either.

![15.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/15.jpg)

So, at this point, I added a small battery block to address this issue.

![16.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/16.jpg)

it worked much better.

![17.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/17.jpg)

: Later on, I added multiple force constraints to ensure the accuracy of the calculation results.

![18.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/18.jpg)

This is the final outcome.

![19.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/19.jpg)

The generated mesh appears rough, likely due to the lower number of simulated faces.

![20.JPG](WeeklyReport004%20a39e71aa9955487e81aee2d8be051cc9/20.jpg)

Now, I'm smoothing the model in Rhino, and I will arrange for printing as soon as possible.