# WekaBayesManager
WekaのEditableBayesNetクラスを簡単に利用できるようにしたクラスです。<br><br>
  WekaBayesManager bayes=new WekaBayesManager("xml/werewolf.xml");<br>
	bayes.setEvidence("seer_role", "possessed");<br>
	bayes.setEvidence("day", "1");<br>
	bayes.clearEvidence("day");<br>
	System.out.println(bayes.getMarginalProbability("species", "human"));<br><br>
このBayesManagerクラスを使用する場合Wekaの導入が必要になります。ビルドパスにweka.jarを追加してください。<br>
このクラスの詳しい説明などは、はjavaファイルのほうを見てください。コメントで書いてあります。
