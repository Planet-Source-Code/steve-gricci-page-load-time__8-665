<div align="center">

## Page Load Time


</div>

### Description

This small script will let you output how much time (in seconds) it took for the page to expell. i.e. 0.501 seconds
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Steve Gricci](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/steve-gricci.md)
**Level**          |Beginner
**User Rating**    |4.6 (87 globes from 19 users)
**Compatibility**  |PHP 3\.0, PHP 4\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__8-1.md)
**World**          |[PHP](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/php.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/steve-gricci-page-load-time__8-665/archive/master.zip)





### Source Code

/*<br>
*@author steve gricci <rejuvenx@deepcode.net><br>
*@access public<br>
*@skill beginner<br>
*@site www.deepcode.net<br>
*/<br><br>
//put at begining of file<br><br>
function utime (){<br>
  $time = explode( " ", microtime());<br>
  $usec = (double)$time[0];<br>
  $sec = (double)$time[1];<br>
  return $sec + $usec;<br>
}<br>
 $start = utime(); <br><br>
//put at end of page before /body and /html tags<br><br>
$end = utime(); $run = $end - $start; echo "Page expelled in " . substr($run, 0, 5) . " secs.";<br>
//Nothing after this

