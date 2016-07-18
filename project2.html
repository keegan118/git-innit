<?php

$list = "BUCKAROO
DWARVES
GIZMO
DAIQUIRI
MICROWAVE
SCHIZOPHRENIA
PNEUMONIA
OXIDIZE
XYLOPHONE
ZEPHYR
ZODIAC
SPHINX
JIUJITSU
HAPHAZARD
KILOBYTE
BAGPIPES
 ";

$alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

echo<<<endHTML
<html>
<head>
<title>Hangman</title>
<style type="text/css">
<!--
h1	{font-family: cursive, monospace; font-size: 50pt;}
p	{font-family: sans-serif; font-size: 15pt;}
body {background-color: gold}
-->
</style>
</head>

<body>
<div align="center">
endHTML;

$length = strlen($alphabet);

if(isset($_GET["n"])) $n=$_GET["n"];
if(isset($_GET["letters"])) $letters=$_GET["letters"];
if(!isset($letters)) $letters="";

if(isset($PHP_SELF)) $self=$PHP_SELF;
else $self=$_SERVER["PHP_SELF"];

$links="";

$max=6;
# error_reporting(0);
$list = strtoupper($list);
$words = explode("\n",$list);
srand ((double)microtime()*1000000);
$all_letters=$letters;
$wrong = 0;

echo "<p font-size: 30><b>Hangman!</b> &nbsp;</b><br>\n";

if (!isset($n)) { $n = rand(1,count($words)) - 1; }
$word_line="";
$word = trim($words[$n]);
$done = 1;
for ($x=0; $x < strlen($word); $x++)
{
  if (strstr($all_letters, $word[$x]))
  {
    if ($word[$x]==" ") $word_line.="&nbsp; "; else $word_line.=$word[$x];
  } 
  else { $word_line.="_<font size=1>&nbsp;</font>"; $done = 0; }
}

if (!$done)
{

  for ($c=0; $c<$length; $c++)
  {
    if (strstr($letters, $alphabet[$c]))
    {
      if (strstr($words[$n], $alphabet[$c])) {$links .= "\n<B>$alphabet[$c]</B> "; }
      else { $links .= "\n<font color=\"light blue\">$alphabet[$c] </font>"; $wrong++; }
    }
    else
    { $links .= "\n<A HREF=\"$self?letters=$alphabet[$c]$letters&n=$n\">$alphabet[$c]</A> "; }
  }
  $nwrong=$wrong; if ($nwrong>6) $nwrong=6;

  echo "\n<p><br>\n<IMG SRC=\"hang_$nwrong.png\" align=\"middle\" border=0 width=500 height=500 alt=\"Wrong: $wrong out of $max\">\n <br><br>";

  if ($wrong >= $max)
  {
    $n++;
    if ($n>(count($words)-1)) $n=0;
    echo "<br><br><h1><font size=5>\n$word_line</font></h1>\n";
    echo "<p><br><font color=\"green\"><big>You're garbage, you lose!</big></font><br><br>";
    if (strstr($word, " ")) $term="phrase"; else $term="word";
    echo "The $term was \"<B>$word</B>\"<br><br>\n";
    echo "<A HREF=$self?n=$n>Play again.</A>\n\n";
  }
  else
  {
    echo " &nbsp; Guesses Remaining: <b>".($max-$wrong)."</b><br>\n";
    echo "<h1><font size=5>\n$word_line</font></h1>\n";
    echo "<p>Choose a letter:<br><br>\n";
    echo "$links\n";
  }
}
else
{
  $n++;	# get next word
  if ($n>(count($words)-1)) $n=0;
  echo "<br><br><h1><font size=5>\n$word_line</font></h1>\n";
  echo "<p><br><br><b>Congratulations!!! &nbsp;You win!!!</b><br><br><br>\n";
  echo "<A HREF=$self?n=$n>Play again</A>\n\n";
}

echo<<<endHTML

</div></body></html>

endHTML;
?>