<h2> Project </h2>
<p>this project demonstrates services to <p>
  <ul>
    <li> convert IFC-SPF to JSON </li>
    <li> 3d-viewer to render the geometry on the browser </li>
    <li> xml based validation using schematron </li>
    <li> using linked-data algorithms to view the IFC </li>
</ul>
<br>
<h2> Prepare your computer/environment </h2>
<p> There are two parts: backend using docker containers and client as node-red flows, provided in this repository</p>
<p> Get the docker container <a href="https://hub.docker.com/repository/docker/nirvik00/ifcproj"> at the docker hub link</a> </p>
<p> Start the docker container as per instructions in the docker-hub site above and note the ports </p>
<p> Get Node red from <a href="https://nodered.org/"> the official site </a> and install it on your computer</p>
<p> Run node-red at port, say, 1880 </p>
<p> Download this repo and from <i>.../services/flows/</i> dir, directly drag and drop the "flows" (json files) into your node-red canvas </p>
<br>
<h2> Run it on your computer </h2>
<br>
<p> To run the node-red functions, except the viewer, we need to configure the filepath and url-port configs in the node-red flows </p>
<p> Data files for demonstration are provided in the <i>services/data</i> file path </p>
<h4> SPF to JSON </h4>
<li> flow: <i>services/flows/spfconv.json</i>
<li> ifc-spf demo file: <i>services/data/spf/wall_door.ifc</i></li>
<li> url: <i> http://localhost:port/u1x/ </i>
<h4> XML based validation </h4>
<li> flow: <i>services/flows/xmlval.json</i>
<li> demo files: </li>
<ol>
  <li> schema file : <i> services/data/sch/medium.sch</i> </li>    
  <li> xml file: <i>services/data/sch/medium.xml</i></li>
</ol>
<li> url: <i> http://localhost:port/u2x/ </i>
<h4> JSON-LD </h4>
<li> flow: <i>services/flows/ld_transform.json</i>
<li> demo files: </li>
<ol>
  <li> document file : <i> services/data/ld/doc.json</i> </li>    
  <li> framing file: <i>services/data/ld/frame.json</i></li>
</ol>
<li> url: <i> http://localhost:port/u3x/ </i>
<h4> Browser based 3d-viewer </h4>
<p> The 3d-viewer can be directly viewed - it takes ifc data from github and renders the building (duplex)</p>
<li> drag and drop the flow: <i>services/flows/viewer.json</i> on your node-red instance running on port, say, 1880</li>
<li> open a new tab on your browser and go to url: <i> http://localhost:1880/x/</i></p>
<li> the ifc data is connected to a Github (remote) end point </li>
