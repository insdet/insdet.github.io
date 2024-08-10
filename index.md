---
layout: default
---
<style> 
.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 75%;
} </style>

# Overview
<div style="text-align: justify">
Instance Detection (InsDet) is an important but fundamental problem in robotics and AR/VR applications. Different from Object Detection (ObjDet) aiming to detect all objects belonging to some predefined classes, InsDet requires detecting specific object instances defined by some examples capturing the instance from multiple views. For example, in a daily scenario, when fetching a specific object instance (e.g., my-coffee-mug), a robot must detect it at a distance, distinguishing it from similar objects (e.g., other mugs or cups) in a cluttered scene for subsequent operations. We invite researchers to the Challenge Workshop on Object Instance Detection where we investigate multiple directions through a competition to address InsDet problem.
<li>A realistic unified InsDet protocol</li> In real-world indoor robotic applications, we consider the scenario that assistive robots must locate and recognize instances to fetch them in a cluttered indoor scene. For a given object instance, the robots should see it only from a few views at the training stage, and then accurately detect it at a distance in any scene at the testing stage. 
<li>InsDet in the closed-world</li> InsDet has been explored in a closed-world setting, which allows access to profile images during model development. While one can exploit profile images to train models, it is still unknown how testing images look like when encountered in the open world. Prevalent methods adopt a cut-paste-learn strategy [10] that cuts and pastes profile images on random background photos (sampled in the open world) to generate synthetic training data and uses such synthetic data to train a detector.
<li>InsDet in the open-world</li> The challenge of InsDet lies in its open-world nature that one has no knowledge of data distribution at test-time, which can be unknown testing scene imagery, unexpected scene clutter, and novel object instances specified only in testing. Prevalent methods exploit the open world by using foundation models [1] and by using diverse data to pretrain InsDet models [3].  
</div>

# Invited Speakers
<div style="display: flex">
    <div style="width:22.5%">
    <a href="https://aimerykong.github.io/">
    <img alt="Shu Kong" src="pics/people/shu.jpg" height="200"  width ="200" style =  "border-radius: 50%; object-fit: cover; ">
    </a><br>
    <a href="https://aimerykong.github.io/">Shu Kong</a><br>
    UMacau, Texas A&M
  </div>
  <div style="width:7.5%">
  </div>
   
  <div style="width:22.5%">
    <a href="https://insdet.github.io/">
    <img alt="TBD" src="pics/people/profile-dummy.jpg"  height="200"   width ="200" style =  "border-radius: 50%; object-fit: cover; ">
    </a><br>
  <a href="https://insdet.github.io/">Dan Parker</a><br>
    TBD
  </div>
  <div style="width:7.5%">
  </div>
  
</div>

## Schedule
<table>
  <tr><td>Times (PDT)</td><td> </td></tr>
  <tr><td>08:30-08:45</td><td>Opening remarks</td></tr>
  <tr><td>08:45-09:25</td><td>Shu Kong, TBD</td></tr>
  <tr><td>09:25-10:05</td><td>TBD, TBD</td></tr>
  <tr><td>10:05-10:10</td><td>Coffee break</td></tr>
  <tr><td>10:10-10:50</td><td>TBD, TBD</td></tr>
  <tr><td>10:50-11:05</td><td>Challenge Overview and Results</td></tr>
  <tr><td>11:05-11:50</td><td>Challenge Winner Talks</td></tr>
  <tr><td>11:50-12:00</td><td>Closing remarks</td></tr>
</table>


## Organizers
<div style="display: flex">
  <div style="width:22.5%">
    <a href="https://shenqq377.github.io/">
    <img alt="Qianqian Shen" src="pics/people/qianqian-shen.png" height="200"  width ="200" style =  "border-radius: 50%; object-fit: cover; ">
    </a><br>
    <a href="https://shenqq377.github.io/">Qianqian Shen</a><br>
    Zhejiang University
  </div>
  
  <div style="width:7.5%">
  </div>
   
  <div style="width:22.5%">
    <a href="https://www.aminer.cn/profile/5617e32a45cedb3397c418c6">
    <img alt="Haishuai Wang" src="pics/people/haishuai-wang.jpg"  height="200"   width ="200" style =  "border-radius: 50%; object-fit: cover; ">
    </a><br>
  <a href="https://www.aminer.cn/profile/5617e32a45cedb3397c418c6">Haishuai Wang</a><br>
    Zhejiang University
  </div>
  
    <div style="width:7.5%">
  </div>
       
  <div style="width:22.5%">
    <a href="https://ics.uci.edu/~yunhaz5/">
    <img alt="Yunhan Zhao" src="pics/people/yunhan-zhao.jpg"   height="200"  width ="200" style =  "border-radius: 50%; object-fit: cover; ">
    </a><br>
  <a href="https://ics.uci.edu/~yunhaz5/">Yunhan Zhao</a><br>
    UC Irvine
  </div>
  
    <div style="width:2.5%">
  </div>

</div>

<div style="display: flex">
  <div style="width:22.5%">
    <a href="https://nahyunkwon.github.io/">
    <img alt="Nahyun Kwon" src="pics/people/profile-dummy.jpg"   height="200" width ="200" style =  "border-radius: 50%; object-fit: cover; ">
    </a><br>
  <a href="https://nahyunkwon.github.io/">Nahyun Kwon</a><br>
    Texas A&M
  </div>
  
    <div style="width:7.5%">
  </div>
  
    <div style="width:22.5%">
    <a href="https://insdet.github.io/">
    <img alt="Kelu Yao" src="pics/people/profile-dummy.jpg"  height="200"  width ="200" style =  "border-radius: 50%; object-fit: cover; ">
    </a><br>
  <a href="https://insdet.github.io/">Kelu Yao</a><br>
    Zhejiang Lab
  </div>

  <div style="width:7.5%">
  </div>


</div>

  
## Challenge

<div style="text-align: justify">
  
  <br>
  This year, we plan to run a competition on our InsDet dataset, which is the first instance detection benchmark dataset which is larger in scale and more challenging than existing InsDet datasets. The major strengths of our InsDet dataset over prior InsDet datasets include (1) both high-resolution profile images of object instances and high-resolution testing images from more realistic indoor scenes, simulating real-world indoor robots locating and recognizing object instances from a cluttered indoor scene in a distance (2) a realistic unified InsDet protocol to foster the InsDet research. Below is a brief description of the competition, including InsDet dataset and benchmark metrics.  

  <div class = "center">
    <img alt="fig2" src="pics/people/profile-dummy.jpg" >
    <p>An illustration of Object Detection vs. Instance Detection.</p>
</div>
  <br>
  The team with the top-performing submission will be invited to give short talks during the workshop.
  <br><br>
</div>


## Important dates
- Challenge start: <strong>9/10/2024</strong>
- Challenge development-phase start: <strong>9/10/2024</strong>
- Challenge test-phase start: <strong>10/20/2024</strong> 
- Challenge close: <strong>11/25/2024</strong>
- Challenge winner announcement: <strong>12/1/2024</strong>
- Workshop day: <strong>12/8/2024</strong>

