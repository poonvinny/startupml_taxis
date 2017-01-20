# startupml_taxis
This is my analysis for the challenge problem portion of the Startup.ml application.  The code uses a sample of T-Drive trajectory dataset that contains one-week trajectories of 10,357 taxis.  

[1] Jing Yuan, Yu Zheng, Xing Xie, and Guangzhong Sun. Driving with knowledge from the physical world. In The 17th ACM SIGKDD international conference on Knowledge Discovery and Data mining, KDD’11, New York, NY, USA, 2011. ACM.

[2] Jing Yuan, Yu Zheng, Chengyang Zhang, Wenlei Xie, Xing Xie, Guangzhong Sun, and Yan Huang. T-drive: driving directions based on taxi trajectories. In Proceedings of the 18th SIGSPATIAL International Conference on Advances in Geographic Information Systems, GIS ’10, pages 99-108, New York, NY, USA,2010. ACM.

GraphDistribution.ipynb goes through the 9 folders the data comes in and produces the distribution of distances and sampling time interval.

SmoothedTrajectory.ipynb picks a trajectory of a particular trip and plots that against a smoothed trajectory.  The trajectory is smoothed using a Rauch-Tung-Striebel Kalman smoother.  The time interval is assumed to be constant to simplify the calculations.  Although this is not the case, the vast majority invervals are at or around the 5 minute mark as evidenced by the time interval plot from GraphDistribution.  

H.E. Rauch, F. Tung, C.T. Striebel.  Maximum Likelihood Estimates of Linear Dynamic Systems.  AIAA Journal Vol.3, No. 8, August 1965.

Mattias Eliasson, A Kalman filter approach to reduce position error for pedestrian applications in areas of bad GPS reception.  
