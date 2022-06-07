<h2> Project </h2>
<p>this project demonstrates services to <p>
  <ul>
    <li>convert IFC-SPF to JSON</li>
    <li>xml based validation using schematron</li>
    <li>using linked-data algorithms to view the IFC </li>
</ul>
<br>
<h2> Run it on your computer </h2>
<p> There are two parts: backend using docker containers and client as node-red flows, provided in this repository</p>
<p> Get the docker container <a href="https://hub.docker.com/repository/docker/nirvik00/ifcproj"> at the docker hub link</a> along with directions and overview </p>
<p> Get Node red from <a href="https://nodered.org/"> the official site </a> and install it on your computer</p>
<p> Run node-red at port, say, 1880 </p>
<p> Download this repo and from <i>.../services/flows/</i> dir, directly drag and drop the "flows" (json files) into your node-red canvas </p>
<p> Start the docker container as per instructions in the docker-hub site above and note the ports </p>
<br>
<p> Overall to run the node-red functions, we need to fix the filepath and url-port configs in the node-red flows </p>
<p> Demo files are provided in the <i>node-red/data</i> file path </p>

<h4> SPF to JSON </h4>
<li> flow: <i>services/flows/spfconv.json</i>
<li> ifc-spf demo file: <i>services/data/spf/wall_door.ifc</i></li>
<li> url: <i> http://localhost:port/u1x/ </i>

<h4> xml Based validation </h4>
<li> ifc-spf demo file: <i>services/data/spf/</i></li>

<h4> JSON </h4>
<li> ifc-spf demo file: <i>services/data/spf</i></li>
