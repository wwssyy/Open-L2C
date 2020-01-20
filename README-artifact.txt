# the HTTP link for docker image of the artifact for this paper

  https://hub.docker.com/repository/docker/yuexincs/cav_2020

# the SHA256 checksum of the artifact file

  63951d027c468ee4f6273fa3119d4d53122d9f64711b563b3ff632cb8b846d26 

# how to build the docker

  1. install docker
  2. docker pull yuexincs/cav_2020
  3. docker run -it yuexincs/cav_2020 bash

# how to build the l2c compiler by yourself 

  Please refer to the README.md file in the source code package, availabe at
         http://soft.cs.tsinghua.edu.cn/~wang/projects/L2C/sources/open-l2c-1.0-Beta.zip
      or https://github.com/wwssyy/Open-L2C/blob/master/open-l2c-1.0-Beta.zip
      or the docker image of the artifact for this paper as above 

# test case path (mentioned in the paper)

  * /root/l2c/test/special/timothy-pldi17/
  * /root/l2c/test/special/paper/tracker_t_sum.lustre, that is, the program shown in Fig.1 of the paper 

# how to run l2c

  l2c <source.lustre>
  then you will get .c file at the path

  eg. l2c /root/l2c/test/special/timothy-pldi17/count/count.LUSTRE
  you will get count.c at /root/l2c/test/special/timothy-pldi17/count/

  particularly, l2c /root/l2c/test/special/paper/tracker_t_sum.lustre  
  you will get tracker_t_sum.c, part of which are shown in Fig.5 and Fig.6 of the paper 

# about software tools in the docker image other than L2C 

  CompCert(v2.6) and GCC(v4.8.4), which are not a part of the artifact for this paper, are also avalable in the docker image. For the usage of CompCert and GCC, it is suggested refering to the related documuents in the official web pages of them. If you have any problem when doing such experiments, please contact us. 
  Email: wwssyy@tsinghua.edu.cn OR yuexin@iscas.ac.cn
