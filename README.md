# WekaBayesManager
WekaのEditableBayesNetクラスを簡単に利用できるようにしたクラスです。<br>
<pre>
    WekaBayesManager bayes=new WekaBayesManager("xml/werewolf.xml");
	bayes.setEvidence("seer_role", "possessed");
	bayes.setEvidence("day", "1");
	bayes.clearEvidence("day");
	System.out.println(bayes.getMarginalProbability("species", "human"));
	</pre>
このBayesManagerクラスを使用する場合Wekaの導入が必要になります。ビルドパスにweka.jarを追加してください。<br>
このクラスの詳しい説明などはjavaファイルのほうを見てください。コメントで書いてあります。
