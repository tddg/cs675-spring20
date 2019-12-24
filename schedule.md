---
layout: page
title: "Course Schedule"
permalink: /schedule.html
---

<style>
table.calendar {
    font-family: arial, helvetica;
    font-size: 10pt;
    empty-cells: show;
    border: 1px solid #000000;
    border-collapse: collapse;
}
table.calendar tr td {
    border: 1px solid #aaaaaa;
}
table.calendar tr {
    vertical-align: top;
    height: 5em;
    background: #ffffff;
}
table.calendar thead tr {
    text-align: center;
    background: #444444;
    color: #ffffff;
    height: auto;
    font-weight: bold;
}
/*.date {
	background: Gainsboro;
}*/
.holiday {
    background: #F0FFF0;
}
.lecture {
    background: #ffffaa;
}
.presentation {
    background: Plum;
}
.exam {
    background: DarkOrange;
}
.important {
    background: #ffaaaa;
}
.nodue {
    background: #ccffcc;
}
.optional {
    background: Linen;
}
.reading {
    color: Black;
}
.deadline {
    background: #ffaaaa;
}
.hwdue {
    color: #ff0000;
	font-weight: bold;
}
.assignment {
    background: #ccffcc;
    color: #0aa00a;
}
.date {
	background: #eeeeee;
    color: #444444;
}
</style>

The course schedule is tentative and subject to change.
<p>
<table class="calendar" cellspacing="0" cellpadding="6" width="100%">
 <thead>
  <tr>
   <td width="10%">Date</td><td width="30%">Topic</td>
   <td width="30%">Required reading/assignment</td><td width="30%">Optional reading</td>
  </tr>
 </thead>

<tr> <!-- week of Jan 20 -->
  <td id="2020-1-22" class="date"><b>Jan 22</b></td>
  <td class="lecture">
	<b>Lec 1:</b> Introduction, <br/> 
		Go systems programming</td>
  <td class="assignment">
	<b><a href="./lab1.html">Lab 1</a></b> assigned</td>
  <td class="optional">XXX</td>
</tr>
<tr> <!-- week of Jan 27 -->
  <td id="2020-1-29" class="date"><b>Jan 29</b></td>
  <td class="lecture">
	<b>Lec 2:</b> Remote procedure call, RPCs in Go</td>
  <td class="deadline">
	<span class="hwdue">Lab setup due</span></td>
  <td class="optional">XXX</td>
</tr>
<tr> <!-- week of Feb 3 -->
  <td id="2020-2-5" class="date"><b>Feb 5</b></td>
  <td class="lecture">
	<b>Lec 3:</b> MapReduce, concurrency in Go</td>
  <td class="deadline">
	<span class="hwdue"><a href="./lab1.html">Lab 1</a> due (Friday Feb 5)</span><br/>
	<span class="reading">MapReduce</span></td>
  <td class="optional">Google File System</td>
</tr>
<tr> <!-- week of Feb 10 -->
  <td id="2020-2-12" class="date"><b>Feb 12</b></td>
  <td class="lecture">
	<b>Lec 4:</b> P-B, time & clock</td>
  <td class="assignment">
	<b><a href="./lab2.html">Lab 2</a></b> assigned<br/>
	<span class="reading">XXX</span></td>
  <td class="optional">XXX</td>
</tr>
<tr> <!-- week of Feb 17 -->
  <td id="2020-2-19" class="date"><b>Feb 19</b></td>
  <td class="lecture">
	<b>Lec 5:</b> 2PC, distributed consensus (Raft)</td>
  <td class="nodue">
	<span class="reading">2PC, Paxos, Raft</span></td>
  <td class="optional">Paxos made live,<br/>
	Chain replication</td>
</tr>
<tr> <!-- week of Feb 24 -->
  <td id="2020-2-26" class="date"><b>Feb 26</b></td>
  <td class="holiday">
	<b>Traveling to FAST</b> (NO CLASS)<br/>
	Hack Day!</td>
  <td class="assignment">
	Project ideas released: Pick your project <br/></td>
  <td></td>
</tr>
<tr> <!-- week of Mar 2 -->
  <td id="2020-3-4" class="date"><b>Mar 4</b></td>
  <td class="exam">
	<b>Midterm exam</b> </td>
  <td class="deadline">
	<span class="hwdue"><a href="./lab2.html">Lab 2</a> due</span></td>
  <td></td>
</tr>
<tr> <!-- week of Mar 9 -->
  <td id="2020-3-11" class="date"><b>Mar 11</b></td>
  <td class="holiday">
	<b>Spring recess</b> (NO CLASS)</td>
  <td class="holiday">Enjoy or catchup?!</td>
  <td></td>
</tr>
<tr> <!-- week of Mar 16 -->
  <td id="2020-3-18" class="date"><b>Mar 18</b></td>
  <td class="lecture">
	<b>Lec 6:</b> Spark (YouTube video)</td>
  <td class="deadline">
	<span class="hwdue">Project proposal due</span><br/>
	<span class="reading">Spark</span></td>
  <td></td>
</tr>
<tr> <!-- week of Mar 23 -->
  <td id="2020-3-25" class="date"><b>Mar 25</b></td>
  <td class="lecture">
	<b>Lec 7:</b> Infrastructure, DC/OS</td>
  <td class="nodue">
	<span class="reading">DC/OS, Borg, Mesos</span></td>
  <td class="optional">Google datacenter workload analysis, Hadoop YARN, Quasar, Omega</td>
</tr>
<tr> <!-- week of Mar 30 -->
  <td id="2020-4-1" class="date"><b>Apr 1</b></td>
  <td class="lecture">
	<b>Lec 8:</b> Cluster scheduling: Late scheduling, Sparrow</td>
  <td class="nodue">
	<span class="reading">Late, Sparrow</span></td>
  <td class="optional">??</td>
</tr>
<tr> <!-- week of Apr 6 -->
  <td id="2020-4-8" class="date"><b>Apr 8</b></td>
  <td class="lecture">
	<b>Lec 9:</b> NoSQL, Memcached</td>
  <td class="nodue">
	<span class="reading">Dynamo, Facebook memcache</span></td>
  <td class="optional">BigTable, Spanner</td>
</tr>
<tr> <!-- week of Apr 13 -->
  <td id="2020-4-15" class="date"><b>Apr 15</b></td>
  <td class="lecture">
	<b>Lec 10:</b> Serverless computing</td>
  <td class="deadline">
	<span class="hwdue">Project checkpoint report due</span><br/>
	<span class="reading">Berkeley's view of Serverless Computing</span></td>
  <td class="optional">OpenLambda, SOCK, Wukong</td>
</tr>
<tr> <!-- week of Apr 20 -->
  <td id="2020-4-22" class="date"><b>Apr 22</b></td>
  <td class="lecture">
	<b>Lec 11:</b> Deep learning</td>
  <td class="nodue">
	<span class="reading">Parameter server, TensorFlow</span></td>
  <td class="optional">MXNet, Ray, Applied ML at Facebook</td>
</tr>
<tr> <!-- week of Apr 27 -->
  <td id="2020-4-29" class="date"><b>Apr 29</b></td>
  <td class="presentation">
	<b>Project presentation</b></td>
  <td></td>
  <td></td>
</tr>
<tr> <!-- week of May 4 -->
  <td id="2020-5-6" class="date"><b>May 6</b></td>
  <td class="exam">
	<b>Final exam (take-home exam)</b></td>
  <td class="deadline">
	<span class="hwdue">Final project report due</span></td>
  <td></td>
</tr>

</table>
