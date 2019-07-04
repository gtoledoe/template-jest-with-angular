pipeline{
	agent any


	stages{
		stage('Main'){
			steps{
				echo 'Definiendo pipeline'
				script{
					def pipe = fileLoader.fromGit('base/main_node','https://github.com/gtoledoe/pipeline_conf_tbk.git', 'master', 'gtoledoe_github')
					pipe.call()
				}
			}
		}
	}
}