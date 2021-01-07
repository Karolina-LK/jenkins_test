node('master'){
	def addg = ''
	
	try{
		currentBuild.result = 'SUCCESS'
	}
	catch(err) {
		currentBuild.result = 'FAILURE'
	}
	finally{
		if(currentBuild.getPreviousBuild() != null && currentBuild.result == currentBuild.getPreviousBuild().result) {
			print(currentBuild?.getPreviousBuild().result)
		}else {
			print("empty value")
		}
	}
	
}