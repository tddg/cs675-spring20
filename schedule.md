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

The course schedule is tentative and subject to change. You can find our reading list [here]({{ site.baseurl }}/reading_list.html).
<p>
<table class="calendar" cellspacing="0" cellpadding="6" width="100%">
 <thead>
  <tr>
   <td width="8%">Date</td><td width="45%">Topic</td>
   <td width="30%">Required reading/assignment</td><td width="17%">Optional reading</td>
  </tr>
 </thead>

<tr> <!-- week of Jan 20 -->
  <td id="2020-1-22" class="date"><b>Jan 22</b></td>
  <td class="lecture">
	<b>Lec 1:</b> Introduction [<a href="./public/lecs/lec1-intro.pdf">slides</a>], <br/> 
		Go systems programming [<a href="./public/lecs/precept1_go_basics.pdf">slides</a>] 
			[<a href="./public/lecs/precept1_go_basics+notes.pdf">slides+notes</a>]</td>
  <td class="assignment">
	[<a href="./public/lecs/precept1_handout.docx">syntax</a>] <br/>
	[<a href="./public/lecs/precept1_handout2.docx">go_systems_programming</a>] <br/>
	[<a href="./public/lecs/precept1_sol.tar.gz">precept1 solutions</a>] <br/>
	<b><a href="https://github.com/cs675-spring20-projs/lab0">Lab 0</a></b> out
	</td>
  <td></td>
</tr>
<tr> <!-- week of Jan 27 -->
  <td id="2020-1-29" class="date"><b>Jan 29</b></td>
  <td class="lecture">
	<b>Lec 2:</b> Remote procedure call, RPCs in Go [<a href="./public/lecs/lec2-rpc.pdf">slides</a>]
			[<a href="./public/lecs/lec2-rpc+notes.pdf">slides+notes</a>]</td>
  <td class="deadline">
	[<a href="./public/lecs/precept2_handout.pdf">wc client+server</a>] <br/>
	<span class="hwdue"><a href="https://github.com/cs675-spring20-projs/lab0">Lab 0</a> due midnight Friday 01/31</span><br/>
	<b><a href="https://git.gmu.edu/cs675-spring20-labs/lab1">Lab 1</a></b> out</td>
  <td></td>
</tr>
<tr> <!-- week of Feb 3 -->
  <td id="2020-2-5" class="date"><b>Feb 5</b></td>
  <td class="lecture">
	<b>Lec 3:</b> MapReduce, concurrency in Go [<a href="./public/lecs/lec3-mr-concurrency.pdf">slides</a>]
		[<a href="./public/lecs/lec3-mr-concurrency+notes.pdf">slides+notes</a>]</td>
  <td class="nodue">
	<span class="reading"><a href="./public/papers/mapreduce_osdi04.pdf">MapReduce</a></span></td>
  <td class="optional"><a href="./public/papers/gfs_sosp03.pdf">Google File System</a><br/>
		Fun read: <a href="https://www.newyorker.com/magazine/2018/12/10/the-friendship-that-made-google-huge">The friendship that made Google huge</a></td>
</tr>
<tr> <!-- week of Feb 10 -->
  <td id="2020-2-12" class="date"><b>Feb 12</b></td>
  <td class="lecture">
	<b>Lec 4:</b> Time & clocks, primary-backup [<a href="./public/lecs/lec4-time-pb.pdf">pdf</a>]
		[<a href="./public/lecs/lec4-time-pb-uploaded.pptx">pptx</a>]
		[<a href="./public/lecs/lec4-time-pb+notes.pdf">pdf+notes</a>]</td>
  <td class="deadline">
	<span class="hwdue"><a href="https://git.gmu.edu/cs675-spring20-labs/lab1">Lab 1</a> due midnight Friday 02/14</span><br/>
	<b><a href="https://git.gmu.edu/cs675-spring20-labs/lab2">Lab 2</a></b> out</td>
  <td></td>
</tr>
<tr> <!-- week of Feb 17 -->
  <td id="2020-2-19" class="date"><b>Feb 19</b></td>
  <td class="lecture">
	<b>Lec 5:</b> Distributed consensus [<a href="./public/lecs/lec5-consensus.pdf">slides</a>] 
		[<a href="./public/lecs/lec5-consensus+notes.pdf">slides+notes</a>],<br/>
		Paxos [<a href="./public/lecs/paxos.pdf">slides</a>] [<a href="./public/lecs/paxos+notes.pdf">slides+notes</a>], <br/>
		Raft [<a href="./public/lecs/raft.pdf">slides</a>]</td>
  <td class="nodue">
	<span class="reading"><a href="./public/papers/paxos_simple.pdf">Paxos made simple</a>, <br/>
		<a href="./public/papers/raft_atc14.pdf">Raft</a></span></td>
  <td class="optional"><a href="./public/papers/paxos_live.pdf">Paxos made live</a>,<br/>
		<a href="./public/papers/chubby_osdi06.pdf">Chubby</a>, <br/>
		<a href="./public/papers/zk_atc10.pdf">Zookeeper</a></td>
</tr>
<tr> <!-- week of Feb 24 -->
  <td id="2020-2-26" class="date"><b>Feb 26</b></td>
  <td class="holiday">
	<b>Traveling to FAST</b> (NO CLASS)<br/>
	<b>Midterm review</b> [<a href="./public/lecs/midterm-review.pdf">slides</a>]<br/>
	...and also, Hack Day!</td>
  <td class="assignment">
	Project ideas released: <a href="./proj.html">Pick your project</a> <br/></td>
  <td></td>
</tr>
<tr> <!-- week of Mar 2 -->
  <td id="2020-3-4" class="date"><b>Mar 4</b></td>
  <td class="exam">
	<b>Midterm exam</b> </td>
  <td class="deadline">
	<span class="hwdue"><a href="https://git.gmu.edu/cs675-spring20-labs/lab2">Lab 2</a> due midnight Wednesday 03/04</span></td>
  <td></td>
</tr>
<tr> <!-- week of Mar 9 -->
  <td id="2020-3-11" class="date"><b>Mar 11</b></td>
  <td class="holiday">
	<b>Spring Recess</b> (NO CLASS)</td>
  <td class="holiday"></td>
  <td></td>
</tr>
<tr> <!-- week of Mar 16 -->
  <td id="2020-3-18" class="date"><b>Mar 18</b></td>
  <td class="holiday">
	<b>Extended Spring Recess</b> (NO CLASS)</td>
  <td class="holiday"></td>
  <td></td>
</tr>
<tr> <!-- week of Mar 23 -->
  <td id="2020-3-25" class="date"><b>Mar 25</b></td>
  <td class="lecture">
	<b>Lec 6:</b> Raft [<a href="./public/lecs/raft.pdf">slides</a>]
			[<a href="./public/lecs/raft+notes.pdf">slides+notes</a>], <br/>  
		Spark [<a href="./public/lecs/lec6-spark.pdf">pdf</a>] 
			  [<a href="./public/lecs/lec6-spark.pptx">pptx</a>]
			  [<a href="./public/lecs/lec6-spark+notes.pdf">pdf+notes</a>] </td>
  <td class="nodue">
	<span class="reading"><a href="./public/papers/spark_nsdi12.pdf">Spark</a></span></td>
  <td class="optional"><a href="./public/papers/ramcloud_tocs15.pdf">RAMCloud</a>, <br/>
		<a href="./public/papers/dryad_eurosys07.pdf">Dryad</a></td>
</tr>
<tr> <!-- week of Mar 30 -->
  <td id="2020-4-1" class="date"><b>Apr 1</b></td>
  <td class="lecture">
	<b>Lec 7:</b> Serverless computing I (background & trends) [<a href="./public/lecs/lec7-serverless-computing-1.pdf">slides</a>]
		[<a href="./public/lecs/lec7-serverless-computing-1+notes.pdf">slides+notes</a>]</td>
  <td class="deadline">
	<span class="hwdue">Project proposal due <strike>Wednesday 04/01</strike> Friday 04/03</span><br/>
	<span class="reading"><a href="./public/papers/berkeley_serverless.pdf">Berkeley's view of serverless computing</a></span></td>
  <td class="optional"><a href="https://www.usenix.org/conference/nsdi20/presentation/agache">Firecracker</a>,
		<a href="https://www.usenix.org/node/196323">OpenLambda</a></td>
</tr>
<tr> <!-- week of Apr 6 -->
  <td id="2020-4-8" class="date"><b>Apr 8</b></td>
  <td class="lecture">
	<b>Lec 8:</b> Serverless computing II (applications) [<a href="./public/lecs/lec8-infinicache.pdf">infinicache_slides</a>]
		[<a href="./public/lecs/lec8-wukong.pdf">wukong_slides</a>]</td>
  <td class="nodue">
	<span class="reading"><a href="https://www.usenix.org/conference/fast20/presentation/wang-ao">InfiniCache</a>,<br/> 
		<a href="https://arxiv.org/abs/1910.05896">Wukong</a></span></td>
  <td class="optional"><a href="https://tddg.github.io/cs675-spring20/public/papers/pywren_socc17.pdf">PyWren</a>
		(<a href="https://arxiv.org/pdf/1810.09679.pdf">numpywren</a>),
		<a href="https://tddg.github.io/cs675-spring20/public/papers/excamera_nsdi17.pdf">ExCamera</a></td>
</tr>
<tr> <!-- week of Apr 13 -->
  <td id="2020-4-15" class="date"><b>Apr 15</b></td>
  <td class="lecture">
	<b>Lec 9:</b> Amazon Dynamo [<a href="./public/lecs/lec9-scale-out-kvs-dynamo.pdf">slides</a>]
		[<a href="./public/lecs/lec9-scale-out-kvs-dynamo+notes.pdf">slides+notes</a>],<br/>
		</td>
  <td class="nodue">
	<span class="reading"><a href="./public/papers/dynamo_sosp07.pdf">Amazon Dynamo</a>,<br/>
		</span></td>
  <td class="optional">
		<a href="./public/papers/bigtable_osdi06.pdf">Google's Bigtable</a>, <br/>
		<a href="./public/papers/chord_sigcomm01.pdf">Chord P2P</a></td>
  <!--td class="lecture">
	<b>Lec 10:</b> Infrastructure, DC/OS</td>
  <td class="deadline">
	<span class="hwdue">Project checkpoint report due Wednesday 04/15</span><br/>
	<span class="reading">DC/OS, Borg, Mesos</span></td>
  <td class="optional">Google datacenter workload analysis, Hadoop YARN, Quasar, Omega</td-->
</tr>
<tr> <!-- week of Apr 20 -->
  <td id="2020-4-22" class="date"><b>Apr 22</b></td>
  <td class="lecture">
	<b>Lec 10:</b> Facebook memcache [<a href="./public/lecs/lec9-fbmc.pdf">slides</a>]
		[<a href="./public/lecs/lec9-fbmc+notes_v2.pdf">slides+notes</a>]</td>
  <td class="nodue">
	<span class="reading"><a href="./public/papers/memcache_nsdi13.pdf">Facebook memcache</a>, <br/>
		<a href="./public/papers/fbkvs_sigmetrics12.pdf">Workload analysis of Facebook's memcache</a></span></td>
  <td></td>
</tr>
<tr> <!-- week of Apr 27 -->
  <td id="2020-4-29" class="date"><b>Apr 29</b></td>
  <td class="lecture">
	<b>Lec 11:</b> Ray RL framework</td>
  <td class="nodue">
	<span class="reading"><a href="./public/papers/ray_osdi18.pdf">Ray</a></span></td>
  <td class="optional">MXNet, TensorFlow, Applied ML at Facebook</td>
</tr>
<tr> <!-- week of May 4 -->
  <td id="2020-5-6" class="date"><b>May 6</b></td>
  <td class="presentation">
	<b>Project presentation</b></td>
  <td class="nodue"></td>
  <td></td>
</tr>
<tr> <!-- week of May 11 -->
  <td id="2020-5-13" class="date"><b>May 13</b></td>
  <td class="exam">
	<b>Final exam (TBD)</b></td>
  <td class="deadline">
	<span class="hwdue">Final project report and src due Friday 05/15</span></td>
  <td></td>
</tr>

</table>
