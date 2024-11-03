java c
EENG6460-Robotics and AI 
Instruction for Experimental Robotics lab 
(Lab No. 2)
1- Objectives of this lab This lab has two sessions. Topics covered during this lab are the Omron robot introduction and safety considerations, Cobot Software (TMFlow) and robot programming, and the robot’s accuracy and repeatability test according to the ISO 9283 standard.There are 6 tasks. So please document the completion of each task by taking pictures/videos, saving any data, and saving the TMFlow code. You will document all results in your final laboratory presentation by submitting a recorded video presentation (maximum 15 minutes) or 15 slides.
2- First Session 
In the first session, you will familiarize yourself with the Omron  robot  introduction,  safety considerations, Cobot Software (TMFlow), and robot programming.
3- Introduction The TM5-900  is  one  of  the  most  compact  robots  that  can  be  easily  integrated into  any production line.  It  has 6  DOF and is designed with a built-in vision system specifically for flexible  production  needs  required  by  small parts  assembly and production processes in consumer electronics and consumer goods (Figure 1).

Figure 1- Omron robotTMflow is the programming system for the Omron robot. It expands the powerful machine vision capabilities of the Omron TM robot to an additional external camera, enabling even more vision guidance and inspection possibilities. For more information please visit:
https://www.youtube.com/watch?v=q7l9BLfLO2E 
https://www.youtube.com/watch?v=7jGXwGiYV3g
4-  Safety and risk assessment 
The main hazards of using industrial robots are divided into three groups: mechanical hazards, human errors and failures.
a-   Mechanical Hazards
Collisions with moving parts or trapping injuries caused by the robot's powerful arms and end- effectors, especially during unexpected movements.
b-  Human Error
Mistakes   made   by   operators,   such   as  programming  errors,   failure   to   follow  safety considerations or unintended proximity to the robot, can lead to accidents.
c-   FailuresMechanical or software malfunctions, such as sensor errors, unanticipated power surges, or communication  breakdowns,  can  cause   uncontrolled  movements  or  failures,   leading  to hazardous situations.
Safety considerations:
The Robot can cause serious injury or death, or damage to itself and other equipment; if the safety precautions are not observed. So please:.     Ensure the workspace is clear of obstacles. The robot’s reach height is 900 mm for the
TM5-900.
.     Do not place any part of your body within the robot's working range while it is powered on.
.     Ensure the emergency stop button is easily accessible from multiple locations around the workspace.Safety and minimising adverse impacts are the most important parameters when working with robots. ISO 10218-1:2011 specifies requirements and guidelines for the inherent safe design, protective measures and information for the use of industrial robots and ISO/TS 15066:2016 specifies  safety  requirements  for  collaborative  industrial  robot  systems  and  the  work environment.
5-  Cobot Software (TMFlow) and robot programming Cobot software, such as TMFlow for Omron's TM series collaborative robots, is designed to simplify  robot  programming  and  operation,   making  it  accessible  even  to   users  without extensive  technical  backgrounds.  TMFlow   utilizes  a  graphical,  flow-based   programming interface that allows users to create robot programs by dragging and dropping function blocks and connecting them to form. a sequence of actions. This intuitive approach eliminates the need for complex coding, enabling users to program robots quickly and efficiently.TMFlow includes a variety of pre-built function blocks for common tasks such as movement commands, logic operations, and input/output control, which can be easily configured to suit specific applications (Figure 2).

Figure 2: TMFlow environmentRobot programming with TMFlow also emphasizes simulation and testing to ensure programs work  as  intended  before  being  executed  on  the  actual  robot.  The  software  provides  a simulation mode where users can visualize and test their programs in a virtual environment, allowing them to identify and correct any issues beforehand. This feature not only enhances the reliability and safety of robot operations but also accelerates the development process. By offering a user-friendly interface and robust simulation capabilities, TMFlow empowers users to harness the full potential of collaborative robots in diverse applications, from manufacturing and assembly to inspection and logistics. Please see the link below before lab starts:
https://www.youtube.com/watch?v=Qi0LJYY_7FU
6-  Tasks to do in the first session Tasks 1-3 are related to the first session and tasks 4-5 are related to the second session. After doing  all  tasks  in  these  two  sessions,  you  need  to  prepare  a  15-minute recorded  video presentation or PowerPoint slides containing tasks 1-5 and upload the video or its link (During the  lab,  do代 写EENG6460-Robotics and AISPSS
代做程序编程语言cument  your  progress  by  screenshots,  write  the  data  gathered,  and  take pictures/videos for your final presentation).
Task 1:
Find the D-H parameters of the robot while discussing with your peers. You can use a ruler.    [20 marks]
Task 2:
A)  Write a program in TMflow so that the robot end effector moves from the base point(PointA) to a point (PonitB) which  is  100  mm  away  in the X direction.  Explain the flowchart of the program that you wrote in the TMFlow environment to make the Omron robot move in X direction. Use steps 1-3.
B)  Change the robot's program to move the end effector in a square-shaped path and a circle path and discuss with your peers the of changing the Motion Setting and Point Management.[20 marks]
Step 1: Creating a robot project 
1.   Open the ‘Project’ screen via the 'Function menu'.
2.   Create a new project, name it ‘Exercise1’.
3.   Open the play book on the 'Simple Motion' page.
4.   Using either ‘free mode’ or the jogging functions, move the robot arm to location A.
5.   Press the ‘POINT’ button on the end effector to save this  point (A point node should be added to the program).
6.   Repeat this process for position B creating a total of 2 points.
7.   Click and drag to create a loop from the ‘last point’ back to the ‘first point’.
8.   Save the project as ‘Exercise1’ when finished.
Step 2: Executing The Project 
1.   Press the ‘PLAY’ button on the robot stick. The program ‘should’ begin to operate.2.   Verify  the  program  moves  the  robot arm to these  programmed  points  (A  to  B),  and
then starts the process again.
3.   Using the ‘+’ and ‘–’ keys on the robot stick, to adjust the speed of the robot.
4.   The ‘View’ screen ‘should’ open automatically when the program is started.
5.   On the ‘Flow page’ , view the program progress as it runs.
6.   On the ‘Simulator’ page, verify the robot is moving according to the program.
7.   Press the ‘STOP’ button on the robot stick to end the program.
8.   The ‘View’ screen ‘should’ close and return automatically to the ‘Project’ screen.
9.   Experiment with both the ‘Step Run’ and ‘Diagnosis’ modes.
Step 3: Modifying Points (Change PTP to Line) 
Using the program from ‘Exercise1’, make the following changes:
1.   Rename each node 'PointA' through to 'PointB' (Using 'Point Manager').
2.   Change all 'point node' to use the ‘line’ move type.
3.   Note that the motion 'icon' (Orange) changes on the point node.
4.   Press the ‘PLAY’ button on the robot stick to test the updated program.
5.   Verify at slow speeds, that the movements are different from in ‘Exercise1’.
6.   Press the ‘STOP’ button when testing has completed.
7.   Save the program as ‘Exercise2’.
Task 3:Explore the robot’s camera and discuss an application when caring for elderly people. How will AI-based robots be user-friendly and safe for all groups of society? Discuss the Ethics, accessibility and inclusiveness.[10 marks]
End of the first lab
7-  Second session of LabThe second session is about the accuracy and repeatability test of the robot according to ISO 9283 standard. Read it and follow the instructions to find the pose accuracy and repeatability of the Omron robot.
8-  Accuracy  and   repeatability  test  of  the robot  according  to   ISO  9283 standardRobot  performance  testing  is  crucial   because  it  ensures  that  a   robot  can   reliably  and accurately perform. its intended tasks in real-world applications. This testing verifies the robot's precision, repeatability, speed, and overall functionality, identifying any potential issues that could affect its operation. ISO 9283 is an international standard that establishes criteria and methods  for  testing  the  performance  of  industrial  robots,  focusing  on  their  accuracy, repeatability,  and  other  key  operational  characteristics.  It  provides  detailed guidelines  for measuring   performance   indicators   such   as   positioning   accuracy,   path   accuracy,   and movement repeatability, ensuring consistent assessment across different robotic systems. By standardizing test conditions, procedures, and measurement techniques, ISO 9283 enables objective   comparisons  of  robot   performance   and   ensures  that   robots   meet   required operational standards, facilitating informed decision-making for manufacturers and users.
Robot Repeatability  Accuracy:
•     Repeatability: positional deviation from the average of displacement.
•     Accuracy: ability to position, at a desired target point within the work volume. Pose accuracy (AP)
•     It  expresses the deviation between a command pose and the mean of the attained poses when approaching the command pose from the same direction.
Pose repeatability (RP)
•     It expresses the closeness of agreement  between the attained poses after n repeat visits to the same command pose in the same direction.The below text is from ISO9283 standard and it will be used in your tasks (See the ISO
9283 standard for more information):







         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
