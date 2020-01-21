<template>
  <div class="jumbotron jumbotron-fluid" style="padding: 0.5em; background-image: url(teren.jpg); background-repeat:no-repeat; background-size:90%; height: 900px; background-position: left">
  <h1 class="display-2" style="font-family:Cuprum; text-align:center; margin-right:100px; color: black; font-size:90px;"><b>1. HNL</b></h1>
  <table style="width: 56%; font-family:Cuprum; font-size:28px; margin-left:320px; color:black; margin-top:30px;">
  <tr>
    <th></th>
    <th></th>
    <th style="font-size:30px; text-align:center; padding-right:100px;">KLUB</th>
    <th style="font-size:30px;">OS</th>
    <th style="font-size:30px;">P</th>
    <th style="font-size:30px;">N</th>
    <th style="font-size:30px;">I</th>
    <th style="font-size:30px;">GZ</th>
    <th style="font-size:30px;">GP</th>
    <th style="font-size:30px;">B</th>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:50px;"> <img src="dinamo.png" width="32px" height="40px"></td>
    <td>Dinamo Zagreb</td>
    <td>19</td>
    <td>15</td>
    <td>2</td>
    <td>2</td>
    <td>36</td>
    <td>8</td>
    <td>47</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:49px;"> <img src="hajduk.png" width="34px" height="34px"></td>
    <td>Hajduk Split</td>
    <td>19</td>
    <td>10</td>
    <td>5</td>
    <td>4</td>
    <td>30</td>
    <td>17</td>
    <td>35</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:51px;"> <img src="rijeka.png" width="28px" height="36px"></td>
    <td>Rijeka</td>
    <td>19</td>
    <td>10</td>
    <td>4</td>
    <td>5</td>
    <td>33</td>
    <td>24</td>
    <td>34</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:53px;"> <img src="osijek.png" width="24px" height="35px"></td>
    <td>Osijek</td>
    <td>19</td>
    <td>9</td>
    <td>6</td>
    <td>4</td>
    <td>34</td>
    <td>22</td>
    <td>33</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:50px;"> <img src="gorica.png" width="32px" height="37px"></td>
    <td>Gorica</td>
    <td>19</td>
    <td>8</td>
    <td>5</td>
    <td>6</td>
    <td>26</td>
    <td>27</td>
    <td>29</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:51px;"> <img src="lokomotiva.png" width="29px" height="38px"></td>
    <td>Lokomotiva Zagreb</td>
    <td>19</td>
    <td>8</td>
    <td>4</td>
    <td>7</td>
    <td>27</td>
    <td>25</td>
    <td>28</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:48px;"> <img src="belupo.png" width="36px" height="36px"></td>
    <td>Slaven Belupo</td>
    <td>19</td>
    <td>5</td>
    <td>3</td>
    <td>11</td>
    <td>18</td>
    <td>35</td>
    <td>18</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:53px;"> <img src="inter.png" width="24px" height="36px"></td>
    <td>Inter Zaprešić</td>
    <td>19</td>
    <td>2</td>
    <td>7</td>
    <td>10</td>
    <td>21</td>
    <td>37</td>
    <td>13</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:45px;"> <img src="istra.svg" width="40px" height="40px"></td>
    <td>Istra 1961</td>
    <td>19</td>
    <td>2</td>
    <td>6</td>
    <td>11</td>
    <td>16</td>
    <td>30</td>
    <td>12</td>
  </tr>
  <tr>
    <td colspan="2" style="padding-left:51px;"> <img src="varazdin.png" width="29px" height="36px"></td>
    <td>Varaždin</td>
    <td>19</td>
    <td>2</td>
    <td>6</td>
    <td>11</td>
    <td>14</td>
    <td>30</td>
    <td>12</td>
  </tr>
</table>

<table style="width: 56%; font-family:Cuprum; font-size:28px; margin-left:320px; color:black; margin-top:100px;">
  <tr>
    <th></th>
    <th></th>
    <th style="font-size:30px; text-align:center; padding-right:100px;">KLUB</th>
    <th style="font-size:30px;">ODIGRANI SUSRETI</th>
    <th style="font-size:30px;">POBJEDE</th>
    <th style="font-size:30px;">NERIJEŠENE</th>
    <th style="font-size:30px;">PORAZI</th>
    <th style="font-size:30px;">BODOVI</th>
  </tr>
  <tr>
    <th></th>
    <th></th>
    <th style="font-size:30px; text-align:center; padding-right:100px;">{{ myteam }}</th>
    <th style="font-size:30px;">{{ played }}</th>
    <th style="font-size:30px;">{{ wins }}</th>
    <th style="font-size:30px;">{{ draws }}</th>
    <th style="font-size:30px;">{{ losses }}</th>
    <th style="font-size:30px;">{{ points }}</th>
  </tr>
  
</table>
  </div>
</template>

<style>
table {
    border: none;
    border-collapse: separate;
    text-align: left;
    border-spacing: 0px;
}
tr:nth-child(even) {background-color: #f2f2f2;}
tr:nth-child(odd) {background-color: #ffffff;}
</style>

<script>
import store from '@/store.js'
export default {
  data(){
    return store;
  }
}
</script>