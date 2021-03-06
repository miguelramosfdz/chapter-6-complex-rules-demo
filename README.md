Chapter 6 - Complex Rules Demo 
=============================
This is an example project for the Effective Business Process Management with JBoss BPM book, 
used in chapter 6. It is a project to automate the installation of the product JBoss BPM Suite 
with preconfigured admin user and sane project defaults along with the complex rules examples
covered in this chapter.


Option 1 - Install on your machine
----------------------------------
1. [Download and unzip.](https://github.com/effectivebpmwithjbossbpm/chapter-6-complex-rules-demo/archive/master.zip)

2. Add product installer to installs directory.

3. Run 'init.sh' or 'init.bat' file. 'init.bat' must be run with Administrative privileges. 

4. Login to http://localhost:8080/business-central  (u:erics / p:bpmsuite1!)

5. Enjoy installed and configured JBoss BPM Suite.


Option 2 - Generate containerized installation
----------------------------------------------
The following steps can be used to configure and run the demo in a container

1. [Download and unzip.](https://github.com/effectivebpmwithjbossbpm/chapter-6-complex-rules-demo/archive/master.zip)

2. Add product installer to installs directory.

3. Build demo image.

	```
	docker build -t effectivebpmwithjbossbpm/chapter-6-complex-rules-demo .
	```
4. Start demo container

	```
	docker run -it -p 8080:8080 -p 9990:9990 effectivebpmwithjbossbpm/chapter-6-complex-rules-demo
	```
5. Login to http://&lt;DOCKER_HOST&gt;:8080/business-central (u:erics / p:bpmsuite1!) 

   ```
   determine DOCKER_HOST with $ docker-machine env
   ```


Released versions
-----------------
See the tagged releases for the following versions of the product:

- v1.0 - JBoss BPM Suite 6.3.0, JBoss EAP 6.4.7 and complex rules examples installed.

![BPM Suite](https://raw.githubusercontent.com/effectivebpmwithjbossbpm/chapter-6-complex-rules-demo/master/docs/demo-images/bpmsuite.png)
