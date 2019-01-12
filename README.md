# PORR_cloudsim
PORR projekt - środowisko CloudSim

Aby odaplić RR mamy 5 plików: 

    1. CircularHostList.java
    2. CloudSimExample9.java (Main Java File)
    3. Hosts.java
    4. RoundRobinDataCenterBroker.java
    5. RoundRobinVmAllocationPolicy.java

Wszystkie wrzuciłem do \PORR_cloudsim\sources\org\cloudbus\cloudsim.
A dodatkowo CloudSimExample9.java wrzuciłem do \PORR_cloudsim\examples\org\cloudbus\cloudsim\examples.

Wszystko odpalamy zgodnie z http://www.cloudbus.org/cloudsim/doc/readme.txt

	"
	3. Installation and running the CloudSim Toolkit
	------------------------------------------------
	
		You just need to unpack the CloudSim file to install.
		If you want to remove CloudSim, then remove the whole cloudsim directory.
		You do not need to compile CloudSim source code. The JAR files are
		provided to compile and to run CloudSim applications:
	
		* jars/cloudsim-<VERSION>.jar                    -- contains the CloudSim class files
		* jars/cloudsim-<VERSION>-sources.jar            -- contains the CloudSim source code files
		* jars/cloudsim-examples-<VERSION>.jar           -- contains the CloudSim examples class files
		* jars/cloudsim-examples-<VERSION>-sources.jar   -- contains the CloudSim examples source code files
	"

I z examples.txt:

	"
	To run the CloudSim examples you need to do the following steps.

	In Windows:

		1. cd <PATH TO CLOUDSIM PACKAGE>\jars
		2. java -classpath cloudsim-<VERSION>.jar;cloudsim-examples-<VERSION>.jar org.cloudbus.cloudsim.examples.CloudSimExample<EXAMPLE NUMBER>

	In Unix/Linux:

		1. cd <PATH TO CLOUDSIM PACKAGE>/jars
		2. java -classpath cloudsim-<VERSION>.jar:cloudsim-examples-<VERSION>.jar org.cloudbus.cloudsim.examples.CloudSimExample<EXAMPLE NUMBER>

	Where you need to replace:

		<PATH TO CLOUDSIM PACKAGE> - by the path to a directory where you have unpacked the CloudSim package
		<VERSION> - by the version of the downloaded CloudSim package
		<EXAMPLE NUMBER> - by the of number of the example you want to run


	CloudSim examples source code
	-----------------------------

	You can find the source code of the examples in <PATH TO CLOUDSIM PACKAGE>/examples/org/cloudbus/cloudsim/examples/


	Compiling and running examples
	------------------------------

	To compile and run an example (let's say org.cloudbus.cloudsim.examples.CloudSimExample1) you need to do the following steps:

	In Windows:

		1. cd <PATH TO CLOUDSIM PACKAGE>
		2. javac -classpath jars\cloudsim-<VERSION>.jar;examples examples\org\cloudbus\cloudsim\examples\CloudSimExample1.java
		3. java -classpath jars\cloudsim-<VERSION>.jar;examples org.cloudbus.cloudsim.examples.CloudSimExample1

	In Unix/Linux:

		1. cd <PATH TO CLOUDSIM PACKAGE>
		2. javac -classpath jars/cloudsim-<VERSION>.jar:examples examples/org/cloudbus/cloudsim/examples/CloudSimExample1.java
		3. java -classpath jars/cloudsim-<VERSION>.jar:examples org.cloudbus.cloudsim.examples.CloudSimExample1


	Compiling and running examples from the power package
	-----------------------------------------------------

	To compile and run an example (let's say org.cloudbus.cloudsim.examples.power.planetlab.LrMc) you need to do the following steps:

	In Windows:

		1. Download Michael Thomas Flanagan's Java Scientific Library from http://www.ee.ucl.ac.uk/~mflanaga/java/
		2. Copy flanagan.jar to <PATH TO CLOUDSIM PACKAGE>/jars/
		3. cd <PATH TO CLOUDSIM PACKAGE>
		4. javac -classpath jars\cloudsim-<VERSION>.jar;jars\flanagan.jar;examples examples\org\cloudbus\cloudsim\examples\power\planetlab\LrMc.java
		5. java -classpath jars\cloudsim-<VERSION>.jar;jars\flanagan.jar;examples org.cloudbus.cloudsim.examples.power.planetlab.LrMc

	In Unix/Linux:

		1. cd <PATH TO CLOUDSIM PACKAGE>
		2. chmod +x ./install-flanagan.sh
		3. ./install-flanagan.jar
		4. javac -classpath jars/cloudsim-<VERSION>.jar:jars/flanagan.jar:examples examples/org/cloudbus/cloudsim/examples/power/planetlab/LrMc.java
		5. java -classpath jars/cloudsim-<VERSION>.jar:jars/flanagan.jar:examples org.cloudbus.cloudsim.examples.power.planetlab.LrMc
	"