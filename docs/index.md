{% include common.html %}
<div class="langlist">
    <span>English</span> |
    <a href="/ja/index.html">日本語</a>
</div>
<div class="movielist">
    <div class="movie">
        <iframe src="https://www.youtube.com/embed/ga61j4KgVss?si=rr6j01WbLRAI3qLg" frameborder="0" allowfullscreen></iframe>
        <br/>
        <span>Purpose</span>
    </div>
    <div class="movie">
        <iframe src="https://www.youtube.com/embed/OFlZLQ8Hy0o?si=C9ZkwMY20SoLbJns" frameborder="0" allowfullscreen></iframe>
        <br/>
        <span>Functionality</span>
    </div>
</div>

## Goal

- Uroboros project was born to revolutionize the conventional robot development method, and aims to accelerate introducing robots into domains where use cases are rather complex for robots to work. We target robots equipped with arms that can freely handle objects and provide a new robot development method that allows you to easily combine any arm with end effectors(tool ​​changer, hand), sensors (camera, force sensor), and conveyance devices (mobile robot, slider, belt conveyor).
- This project mainly aims to help the following people (see video for details)
  - Software developer for robots (e.g. software vendors, AI ventures)
  - Those who conceptualize, develop, and introduce robot systems according to requests (e.g. SIers, user companies)
  - Provider of robot components (e.g. equipment vendors)
  - Researcher on advanced technology for robots (e.g. research institutions)

### 1. Data driven: solution that gives us flexibility
- Conventional arm robots were mostly used for automation by performing predetermined repetitive movements where the environment had been prepared in advance (e.g. factories). On the other hand, for example, when stocking items at a retail store, conventional robots often faces difficulties: there are many types of objects, there is randomness in the position, orientation, and type of objects, and the types of objects change frequently.
- Creating a robot that can move in such an environment is practically impossible using conventional methods. This is because with conventional methods, it is necessary to teach the robot how to grasp and handle each object individually, which incurs development costs each time. In use cases where there are many types of products, the supply pattern is complex, or new products are added frequently, we had no choice but to give up on introducing robots due to the enormous development costs and development time.
- In recent years, systems that use AI to handle multiple types of objects without teaching each object individually have begun to appear, but the mainstream method that does not have a database of objects (cf. model-free method), there is a problem that it is difficult to handle objects accurately.
- Uroboros project believes that the key to solving this problem is data driven robotics that utilizes AI and databases. By storing the information necessary to grasp and handle objects in a database and processing that data with AI, arm-equipped robots that can **"grasp any object and handle accurately"** like a human will be realized. 

### 2. Reusable software
- Additionally, in order to reduce software development costs, which account for most of the development costs for advanced robots, we believe that it is essential to improve software reusability. Currently, software for robots is often developed from scratch for each individual system as a one-off item, and there is little progress in reusing software. One of the reasons for this is that software-hardware interfaces have not been standardized, so that if you try to use robot parts from a different manufacturer, you have to rewrite the software.
- In uroboros project, by providing **drivers for accessing robot parts using a common IF** , we will make it possible to apply the software once created to parts from another manufacturer without change. Uroboros project also promotes **modularization by defining IFs between software parts**. By creating such environment where software can be easily reused and people with different knowledge can share roles and contribute to the creation of advanced systems, we realise a eco-system where the number of companies providing software solutions for robots will increase, software costs lower, and its quality higher compared to one-by-one development.

### 3. Open
- To accelerate developing such smart robots, we believes that databases and a standard framework need to be made available to everyone as **a platform shared by society (robot infrastructure)**. The uroboros project will be carried out on a non-profit basis with support from the robotics industry and NEDO.
- Deliverables of uroboros project will be released as OSS that can be used commercially. We provide a new development option for companies doing business in the robot industry to create new solutions or robot systems by using uroboros as a core and adding or changing necessary elements as needed.

## Deliverables
- To achive our goal, we are mainly developing 2 systems
  - Uroboros cloud: open database system for robotics on cloud
  - Uroboros connect: AI&database-friendly task-oriented robot framework on ROS2
- 開発範囲
  - Uroboros connect is a reference for robot system implementation that utilizes data from uroboros cloud. Uroboros connect provides core implementations such as IF definitions for various software modules to work together and abstraction bridge/utility implementations to improve software reusability, but the following are not provided:
    - Not provided directly
      - Software modules such as drivers that control specific processing for robot operations and various robot parts
      - Points of contact with robot users, or UI for operation.
    - The above must be prepared by each developer (software vendor/parts manufacturer/SIer, etc.)
    - Cataloging to enable easy exploration and combination of software modules is supported by uroboros cloud.
  - For details, please refer to the document that will be released in the future.
- Progress
  - System designs were drafted, and are being revised continuously based on feedback
  - Currently, software implementation and database creation is on-going

## Project Member

- Developers

<div class="logolist">
  <img src="/logo/robocip.svg">
  <img src="/logo/aist.gif">
  <img src="/logo/tsukuba.png">
  <img src="/logo/osaka.png">
  <img src="/logo/tokyo.webp">
  <img src="/logo/okayama.jpg">
  <img src="/logo/musashino.jpg">
</div>

## Acknowledgement
- Uroboros project is supported by NEDO
  - [NEDO project page](https://www.nedo.go.jp/activities/ZZJP_100188.html)

## Contact

- Please contact us if you are interested
  - ROBOCIP uroboros project team
  - pj1db-support@robocip.or.jp