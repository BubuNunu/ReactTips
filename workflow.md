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
* constructer(props)
* 2> ComponentDidMount(d3 to visualize)
* 3> props changes => ComponentWillReceiveProps(update 2>)
* 4> Render

