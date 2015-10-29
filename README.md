# WekaBayesManager
WekaのEditableBayesNetクラスを簡単に利用できるようにしたクラスです。<br>
<pre>
WekaBayesManager bayes=new WekaBayesManager("xml/werewolf.xml");
bayes.setEvidence("seer_role", "possessed");
bayes.setEvidence("day", "1");
bayes.clearEvidence("day");
bayes.calcMargin();
System.out.println(bayes.getMarginalProbability("species", "human"));
</pre>
このBayesManagerクラスを使用する場合Wekaの導入が必要になります。ビルドパスにweka.jarを追加してください。
weka.jarは[Weka-jp.info](http://www.weka-jp.info/index.php/weka-jp/2011-05-25-10-58-08 "Weka-jp.info")
のその他のプラットフォーム(Linuxなど)の項目にあるweka-3-6-10.zipにあります。
このクラスの詳しい説明などはjavaファイルを見てください。コメントで書いてあります。
