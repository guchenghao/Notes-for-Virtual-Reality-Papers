# Paper Link
---

TIME: 2016/09 SAICSIT

[A System for a Hand Gesture-Manipulated Virtual Reality Environment](https://dl.acm.org/doi/10.1145/2987491.2987511)


TIME: 2020/09 SAICSIT

[A system for pose analysis and selection in virtual reality environments](https://dl.acm.org/doi/10.1145/3410886.3410909)

# Problem
---

## purpose

- **limited research** has investigated machine learning techniques for HGR in virtual reality applications (VR).
  
- A review of current literature has revealed that many researchers have used the LMC to classify Sign Language gestures, but very few have applied it to VR.
---

## propose
- This paper reports on the design, implementation, and evaluation of **a static HGR system for VR applications using the LMC**. 
  
- The gesture recognition system incorporated **a lightweight feature vector of five normalized tip-to-palm distances and a k-nearest neighbor (kNN) classifier**.
  
- The system was evaluated in terms of **response time, accuracy and usability using a case-study** VR stellar data visualization application created in the Unreal Engine 4.
  
- This system was created to explore the efficacy of machine learning techniques for HGR in VR applications
---

# Method or Solution
---

## Device and Development tools
- Leap Motion Controller(LMC)
- Unreal Engine4
- Oculus Rift DK2
---

## Steps and models
1. *Data Input*: Collect and read frame data from the LMC
   
2. *Static Gesture Recognition System*: According to step(1), Normalized the LMC input TPP distances data and dataset TPP distances data(Already exist).Then, use **KNN classification algorithm** to classify the static gesture.
   
3. *VR Gesture Handler*: The gesture handler is a component embedded in the application that receives a classified gesture and performs the appropriate action on the VR environment.(**use a finite state machine to divide each hand gesture into a state**)
   
4. *VR Stellar Data Visualization Application*
---

# Experiment
---

- *preliminary User Study*: Three new users, two men and a woman of varying hand
sizes, were included in the study to **measure the ease of use and comfort of the system**.

---

# Result and Conclusion
---

- the system is **lightweight enough** to allow the program to run at a **high framerate**, which is an important consideration to take when developing for VR.
  
- Static gestures used in the application had an 82.5% accuracy rate, with a minimum of 60% accuracy with the point gesture and a maximum of 100% accuracy with the fist gesture.
  
- Gestures with low accuracy ratings primarily suffered from **occlusion issues**
---

# Comment
---

1. ???????????????????????????????????????????????????????????????????????????????????????????????????
   
2. ????????????**???????????????????????????????????????????????????????????????????????????????????????**???????????????HGR????????????????????????VR???????????????????????????????????????????????????????????????(???????????????LMc??????VR???????????????)??????**??????HGR?????????VR??????????????????(????????????)**?????????????????????????????????
   
3. ???????????????user study?????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????
   
4. ???????????????classification???????????????????????????????????????????????????????????????
   
5. ???????????????????????????????????????????????????????????????**????????????**?????????????????????????????????lightweight(?????????)????????????????????????VR????????????????????????????????????KNN????????????????????????????????????
   
6. ???A system for pose analysis and selection in virtual reality environments?????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????gesture recognition???classification????????????????????????????????????????????????????????????????????????**??????????????????????????????????????????????????????pose dataset**???
---

# What can be used
---

- lightweight????????????????????????????????????????????????????????????????????????????????????????????????
  
- ???????????????????????????ML?????????VR??????????????????????????????????????????????????????

- ????????????????????????hand-pose ?????? hand-gesture?????????????????????????????????????????????????????????
