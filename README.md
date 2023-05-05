Download Link: https://assignmentchef.com/product/solved-cse225-project-1-text-representation-with-binary-trees
<br>



In text classification studies, textual materials are represented with the frequencies of the words. Suppose that Table 1 gives the frequencies of 50 words in a document.

Table 1. Frequencies of words in the document

<table width="266">

 <tbody>

  <tr>

   <td width="75"><strong>Number </strong></td>

   <td width="95"><strong>Word </strong></td>

   <td width="95"><strong>Frequency </strong></td>

  </tr>

  <tr>

   <td width="75">1</td>

   <td width="95">people</td>

   <td width="95">6</td>

  </tr>

  <tr>

   <td width="75">2</td>

   <td width="95">country</td>

   <td width="95">10</td>

  </tr>

  <tr>

   <td width="75">3</td>

   <td width="95">city</td>

   <td width="95">15</td>

  </tr>

  <tr>

   <td width="75">4</td>

   <td width="95">news</td>

   <td width="95">2</td>

  </tr>

  <tr>

   <td width="75">5</td>

   <td width="95">population</td>

   <td width="95">1</td>

  </tr>

  <tr>

   <td width="75">6</td>

   <td width="95">society</td>

   <td width="95">28</td>

  </tr>

  <tr>

   <td width="75">7</td>

   <td width="95">university</td>

   <td width="95">35</td>

  </tr>

  <tr>

   <td width="75">8</td>

   <td width="95">sports</td>

   <td width="95">62</td>

  </tr>

  <tr>

   <td width="75">9</td>

   <td width="95">economics</td>

   <td width="95">4</td>

  </tr>

  <tr>

   <td width="75">10</td>

   <td width="95">book</td>

   <td width="95">89</td>

  </tr>

  <tr>

   <td width="75">11</td>

   <td width="95">library</td>

   <td width="95">3</td>

  </tr>

  <tr>

   <td width="75">12</td>

   <td width="95">computer</td>

   <td width="95">7</td>

  </tr>

  <tr>

   <td width="75">13</td>

   <td width="95">mouse</td>

   <td width="95">16</td>

  </tr>

  <tr>

   <td width="75">14</td>

   <td width="95">memory</td>

   <td width="95">27</td>

  </tr>

  <tr>

   <td width="75">15</td>

   <td width="95">game</td>

   <td width="95">50</td>

  </tr>

  <tr>

   <td width="75">16</td>

   <td width="95">student</td>

   <td width="95">60</td>

  </tr>

  <tr>

   <td width="75">17</td>

   <td width="95">club</td>

   <td width="95">70</td>

  </tr>

  <tr>

   <td width="75">18</td>

   <td width="95">text</td>

   <td width="95">83</td>

  </tr>

  <tr>

   <td width="75">19</td>

   <td width="95">algorithm</td>

   <td width="95">46</td>

  </tr>

  <tr>

   <td width="75">20</td>

   <td width="95">compiler</td>

   <td width="95">44</td>

  </tr>

  <tr>

   <td width="75">21</td>

   <td width="95">excel</td>

   <td width="95">49</td>

  </tr>

  <tr>

   <td width="75">22</td>

   <td width="95">name</td>

   <td width="95">51</td>

  </tr>

  <tr>

   <td width="75">23</td>

   <td width="95">department</td>

   <td width="95">56</td>

  </tr>

  <tr>

   <td width="75">24</td>

   <td width="95">head</td>

   <td width="95">54</td>

  </tr>

  <tr>

   <td width="75">25</td>

   <td width="95">faculty</td>

   <td width="95">22</td>

  </tr>

  <tr>

   <td width="75">26</td>

   <td width="95">teacher</td>

   <td width="95">33</td>

  </tr>

  <tr>

   <td width="75">27</td>

   <td width="95">professor</td>

   <td width="95">100</td>

  </tr>

  <tr>

   <td width="75">28</td>

   <td width="95">room</td>

   <td width="95">201</td>

  </tr>

  <tr>

   <td width="75">29</td>

   <td width="95">lab</td>

   <td width="95">92</td>

  </tr>

  <tr>

   <td width="75">30</td>

   <td width="95">kitchen</td>

   <td width="95">94</td>

  </tr>

  <tr>

   <td width="75">31</td>

   <td width="95">clock</td>

   <td width="95">97</td>

  </tr>

  <tr>

   <td width="75">32</td>

   <td width="95">class</td>

   <td width="95">93</td>

  </tr>

  <tr>

   <td width="75">33</td>

   <td width="95">board</td>

   <td width="95">64</td>

  </tr>

  <tr>

   <td width="75">34</td>

   <td width="95">pencil</td>

   <td width="95">65</td>

  </tr>

  <tr>

   <td width="75">35</td>

   <td width="95">window</td>

   <td width="95">61</td>

  </tr>

  <tr>

   <td width="75">36</td>

   <td width="95">team</td>

   <td width="95">19</td>

  </tr>

  <tr>

   <td width="75">37</td>

   <td width="95">software</td>

   <td width="95">13</td>

  </tr>

  <tr>

   <td width="75">38</td>

   <td width="95">group</td>

   <td width="95">14</td>

  </tr>

  <tr>

   <td width="75">39</td>

   <td width="95">grade</td>

   <td width="95">26</td>

  </tr>

  <tr>

   <td width="75">40</td>

   <td width="95">meeting</td>

   <td width="95">88</td>

  </tr>

  <tr>

   <td width="75">41</td>

   <td width="95">bag</td>

   <td width="95">99</td>

  </tr>

  <tr>

   <td width="75">42</td>

   <td width="95">television</td>

   <td width="95">205</td>

  </tr>

  <tr>

   <td width="75">43</td>

   <td width="95">visit</td>

   <td width="95">300</td>

  </tr>

  <tr>

   <td width="75">44</td>

   <td width="95">Ankara</td>

   <td width="95">74</td>

  </tr>

  <tr>

   <td width="75">45</td>

   <td width="95">New York</td>

   <td width="95">77</td>

  </tr>

  <tr>

   <td width="75">46</td>

   <td width="95">Dubai</td>

   <td width="95">76</td>

  </tr>

  <tr>

   <td width="75">47</td>

   <td width="95">plane</td>

   <td width="95">41</td>

  </tr>

  <tr>

   <td width="75">48</td>

   <td width="95">traffic</td>

   <td width="95">42</td>

  </tr>

  <tr>

   <td width="75">49</td>

   <td width="95">car</td>

   <td width="95">43</td>

  </tr>

  <tr>

   <td width="75">50</td>

   <td width="95">bus</td>

   <td width="95">75</td>

  </tr>

 </tbody>

</table>







<ol>

 <li>Build a BST with the key “Word”.</li>

</ol>




<ol>

 <li>Suppose that the number of accesses to word in your tree is directly the frequency of the word given in the table.</li>

</ol>




Calculate Total Access Time in the tree you build in (a).




<ol>

 <li>Suppose that the number of accesses to word in your tree is directly the frequency of the word given in the table. Construct a BT to keep these records in the main memory so as to <strong>minimize the total access time</strong>, where one time unit is the time taken to compare the key of a tree with the key searched!</li>

</ol>




<ol>

 <li>Calculate Total Access Time in the tree you build in (c).</li>

</ol>







<ol>

 <li>Discuss your results in (b) and (d).</li>

</ol>

<strong> </strong>

<strong>VERY IMPORTANT </strong>

<strong>The main goal of this project is to be familiar with trees. So, use of arrays/linked lists instead of trees is not acceptable. </strong>

In this project, you are expected to develop an algorithm that is capable of finding a solution to the above problem and <strong><em>implement this algorithm in ANSI C that runs under either UNIX or Windows</em></strong>.


