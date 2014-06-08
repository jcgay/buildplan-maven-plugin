#buildplan-maven-plugin

A Maven 3.x plugin to inspect the lifecycle of your project.

###Usage

Activate the plugin group in your Maven *settings.xml*:

	<pluginGroups>
	    <pluginGroup>fr.jcgay.maven.plugins</pluginGroup>
  	</pluginGroups>

###List plugin executions within a project
	mvn buildplan:list
	
###List plugin executions within phases
	mvn buildplan:list-phase
It is possible to limit the list to a specific phase:
	
	mvn buildplan:list-phase -Dbuildplan.phase=test
	
###List plugin executions by plugins
	mvn buildplan:list-plugin
It is possible to limit the list to a specific plugin:

	mvn buildplan:list-plugin -Dbuildplan.plugin=maven-compiler-plugin

[Plugin documentation](http://buildplan.jcgay.fr/)
