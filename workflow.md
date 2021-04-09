### 1. lifecyle
<img width = 60% src = "./images/lifeCycle.png">

### 2. Templete
link: https://github.com/xietiankai/create-fullstack-vis-app

### 3. Structure of React
0> prerequisite: Docker </br>
1> The above link is the container of the React platform. </br>
* FrontEnd: React(props: static, state: dynamic), Ant Design
* BackEnd:  Python
</br>
3> To control the global variable, use "React-Redux".
4> workfolow
<pre>
# 0: run the container in the docker.
docker-compose up
# 1: 
# app.js(tell "Base" to load data and go to the layout of the interface "Main") -> 
# components -> action(intermedia to transform data to backend) -> Server
</pre>
</br>
5> Content of Component </br>

* 1> constructer(props)
* 2> ComponentDidMount(d3 to visualize)
* 3> props changes => ComponentWillReceiveProps(update 2>)
* 4> Render

### 4. Run the container
* check the version of Ubuntu
<pre>
# in the terminal
lsb_release -a
# release the info
No LSB modules are available.
Distributor ID:	Ubuntu
Description:	Ubuntu 20.04.2 LTS
Release:	20.04
Codename:	focal
</pre>
* install docker
<pre>
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io
# configure docker to start on boot
sudo systemctl enable docker.service
sudo systemctl enable containerd.service
</pre>
* install docker-compose
<pre>
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
</pre>
* In the container, npm install under gui
<pre>
sudo npm install
</pre>
* start the contanair
<pre>
sudo docker-compose up
</pre>

