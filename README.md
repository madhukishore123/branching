# branching stategry
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
			<title>Excel To HTML using codebeautify.org</title>
		</head>
		<body>
			<!DOCTYPE html>
			<Title>branching stategry</Title>
			<html>
				<body>
					<h1>Master Branch: </h1>
					<p> Master must contain well tested code, application release happens from this branch by     
  creating a release ‘tag’.
  In real world no one directly work on master.</p>
					<h1>Hotfixs Branch: </h1>
					<p>This branch is used for fixing production defects.
   Hotfixes branch is created from master</p>
					<h1>Develop Branch</h1>
					<p>This branch belongs to a specific team, code integration of this team members are 
  done on this branch
Develop branch is created from master</p>
					<h1>Feature Branch</h1>
					<p> Belongs to a specific developer, where his feature in implemented, after completion of 
  a feature changes are merged into his develop branch.
  Feature branch is created from develop branch.The core idea behind the Feature Branch Workflow is that all feature development should take place in a dedicated branch instead of the master branch. This encapsulation makes it easy for multiple developers to work on a particular feature without disturbing the main codebase. It also means the master branch will never contain broken code, which is a huge advantage for continuous integration environments</p>
					<h1>Release Branch</h1>
  This branch is to integrate changes done by multiple teams under their develop branch 

<h1>Branching Strategy Workflow</h1>

<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
			<title>Excel To HTML using codebeautify.org</title>
		</head>
		<body>
			<!DOCTYPE html>
			<html>
				<head>
					<style>
img { 
    width:100%; 
}
</style>
				</head>
				<body>
					<img src="http://nvie.com/img/git-model@2x.png" alt="HTML5 Icon" >
					<img src="http://www.continuousautomation.com/wp-content/uploads/2014/08/scarybranchdiagram.png" alt="HTML5 Icon" style="width:128px;height:128px;">
						
            <img src="https://image.slidesharecdn.com/branchingstrategies-141022194356-conversion-gate01/95/branching-strategies-for-git-and-subversion-8-638.jpg?cb=1414513053">
						</body>
					</html>
				</body>
			</html>

<!DOCTYPE html>
<html>
<head>
<title></title>
</head>
<body>

<h1>WHY GIT?</h1>
<p>the pros and cons of Git compared to centralized source code control system.There are plenty of flame wars going on there.Git really changed the way developers think of merging and branching. From the classic CVS/Subversion world I came from, merging/branching has always been considered a bit scary.But with Git, these actions are extremely cheap and simple, and they are considered one of the core parts of your daily workflow</p>

<h1>Decentralized but centralized </h1>

<p><br>The repository setup that we use and that works well with this branching model, is that with a central “truth” repo. Note that this repo is only considered to be the central one (since Git is a DVCS, there is no such thing as a central repo at a technical level). We will refer to this repo as origin, since this name is familiar to all Git users.Each developer pulls and pushes to origin. But besides the centralized push-pull relationships, each developer may also pull changes from other peers to form sub teams. 
	</br></p>
	
	<h3>Work flow Diagram</h3>
	
	
	<img src="http://nvie.com/img/centr-decentr@2x.png">
	
	<br></br>
	<h1>The main branches </h1>
	<br></br>
	<p>At the core, the development model is greatly inspired by existing models out there. The central repo holds two main branches with an infinite lifetime:</p>
	<br>-MAster</br>
	<br>-Develop</br>
	
	<p><br>The master branch at origin should be familiar to every Git user. Parallel to the master branch, another branch exists called develop.</br>

<br>We consider origin/master to be the main branch where the source code of HEAD always reflects a production-ready state.</br>

<br>We consider origin/develop to be the main branch where the source code of HEAD always reflects a state with the latest delivered development changes for the next release. Some would call this the “integration branch”. This is where any automatic nightly builds are built from.</br>

<br>When the source code in the develop branch reaches a stable point and is ready to be released, all of the changes should be merged back into master somehow and then tagged with a release number. How this is done in detail will be discussed further on<br></p>

<img src="http://nvie.com/img/main-branches@2x.png">
<h1></h1>
</body>
</html>
  
  
