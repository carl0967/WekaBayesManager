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
このBayesManagerクラスを使用する場合Wekaの導入が必要になります。ビルドパスにweka.jarを追加してください。<br>
weka.jarは[Weka-jp.info](http://www.weka-jp.info/index.php/weka-jp/2011-05-25-10-58-08 "Weka-jp.info")
のその他のプラットフォーム(Linuxなど)の項目にあるweka-3-6-10.zipにあります。<br>
WekaBayesManagerの詳しい使い方はjavaファイルを見てください。コメントで書いてあります。<br>

[作成者のブログ](http://informationstudent.blog.fc2.com/blog-entry-26.html "WekaのEditableBayesNetを使いやすくするクラスを作成")
