## Real-Time Bidding by Reinforcement Learning in Display Advertising


## Small-Scale Evaluation Demo
For the demo of the small-scale evaluation, please run under the folder of **scripts**:
```bash
$ bash small-scale.sh
```
or run under the folder of **python**:
```bash
$ python3 bid_ss.py
```
After running, you could get the performance table printed in the console like:
```
setting                                                	  objective	  auction	 impression	    click	     cost	  win-rate	      CPM	     eCPC
ipinyou, camp=1458, algo=ss_mdp, N=1000, c0=0.03125    	         11	   350000	      52757	       11	   748502	    15.07%	    14.19	    68.05
ipinyou, camp=1458, algo=mcpc, N=1000, c0=0.03125      	        121	   350000	      29312	      121	   752015	     8.37%	    25.66	     6.21
ipinyou, camp=1458, algo=lin_bid, N=1000, c0=0.03125   	        243	   350000	      30152	      243	   564282	     8.61%	    18.71	     2.32
ipinyou, camp=1458, algo=rlb, N=1000, c0=0.03125       	        271	   350000	      26292	      271	   687794	     7.51%	    26.16	     2.54
ipinyou, camp=2259, algo=ss_mdp, N=1000, c0=0.03125    	          7	   350000	      63217	        7	  1008842	    18.06%	    15.96	   144.12
ipinyou, camp=2259, algo=mcpc, N=1000, c0=0.03125      	          7	   350000	      19571	        7	  1017600	     5.59%	    52.00	   145.37
ipinyou, camp=2259, algo=lin_bid, N=1000, c0=0.03125   	          8	   350000	      42781	        8	  1002204	    12.22%	    23.43	   125.28
ipinyou, camp=2259, algo=rlb, N=1000, c0=0.03125       	         11	   350000	      46621	       11	  1001535	    13.32%	    21.48	    91.05
ipinyou, camp=2261, algo=ss_mdp, N=1000, c0=0.03125    	          9	   343862	      81995	        9	   960409	    23.85%	    11.71	   106.71
ipinyou, camp=2261, algo=mcpc, N=1000, c0=0.03125      	          7	   343862	      25217	        7	   963167	     7.33%	    38.20	   137.60
ipinyou, camp=2261, algo=lin_bid, N=1000, c0=0.03125   	          8	   343862	      53249	        8	   912583	    15.49%	    17.14	   114.07
ipinyou, camp=2261, algo=rlb, N=1000, c0=0.03125       	         10	   343862	      59163	       10	   961293	    17.21%	    16.25	    96.13
ipinyou, camp=2821, algo=ss_mdp, N=1000, c0=0.03125    	         19	   350000	      65310	       19	   968224	    18.66%	    14.83	    50.96
ipinyou, camp=2821, algo=mcpc, N=1000, c0=0.03125      	         10	   350000	      21217	       10	   976485	     6.06%	    46.02	    97.65
ipinyou, camp=2821, algo=lin_bid, N=1000, c0=0.03125   	         19	   350000	      39136	       19	   753469	    11.18%	    19.25	    39.66
ipinyou, camp=2821, algo=rlb, N=1000, c0=0.03125       	         23	   350000	      49261	       23	   964767	    14.07%	    19.58	    41.95
ipinyou, camp=2997, algo=ss_mdp, N=1000, c0=0.03125    	         80	   156063	      40395	       80	   306637	    25.88%	     7.59	     3.83
ipinyou, camp=2997, algo=mcpc, N=1000, c0=0.03125      	         48	   156063	      14752	       48	   307751	     9.45%	    20.86	     6.41
ipinyou, camp=2997, algo=lin_bid, N=1000, c0=0.03125   	         71	   156063	      32208	       71	   203610	    20.64%	     6.32	     2.87
ipinyou, camp=2997, algo=rlb, N=1000, c0=0.03125       	         78	   156063	      39680	       78	   304375	    25.43%	     7.67	     3.90
ipinyou, camp=3358, algo=ss_mdp, N=1000, c0=0.03125    	          9	   300928	      34289	        9	   857285	    11.39%	    25.00	    95.25
ipinyou, camp=3358, algo=mcpc, N=1000, c0=0.03125      	         81	   300928	      12424	       81	   867133	     4.13%	    69.79	    10.71
ipinyou, camp=3358, algo=lin_bid, N=1000, c0=0.03125   	        202	   300928	       8465	      202	   517007	     2.81%	    61.08	     2.56
ipinyou, camp=3358, algo=rlb, N=1000, c0=0.03125       	        212	   300928	      12970	      212	   836097	     4.31%	    64.46	     3.94
ipinyou, camp=3386, algo=ss_mdp, N=1000, c0=0.03125    	          6	   350000	      51384	        6	   834115	    14.68%	    16.23	   139.02
ipinyou, camp=3386, algo=mcpc, N=1000, c0=0.03125      	         15	   350000	      17839	       15	   840473	     5.10%	    47.11	    56.03
ipinyou, camp=3386, algo=lin_bid, N=1000, c0=0.03125   	         37	   350000	       9279	       37	   213219	     2.65%	    22.98	     5.76
ipinyou, camp=3386, algo=rlb, N=1000, c0=0.03125       	         39	   350000	      29142	       39	   830911	     8.33%	    28.51	    21.31
ipinyou, camp=3427, algo=ss_mdp, N=1000, c0=0.03125    	          4	   350000	      52338	        4	   879547	    14.95%	    16.81	   219.89
ipinyou, camp=3427, algo=mcpc, N=1000, c0=0.03125      	         48	   350000	      19622	       48	   885400	     5.61%	    45.12	    18.45
ipinyou, camp=3427, algo=lin_bid, N=1000, c0=0.03125   	        160	   350000	      17664	      160	   679864	     5.05%	    38.49	     4.25
ipinyou, camp=3427, algo=rlb, N=1000, c0=0.03125       	        171	   350000	      21678	      171	   851729	     6.19%	    39.29	     4.98
ipinyou, camp=3476, algo=ss_mdp, N=1000, c0=0.03125    	         17	   350000	      51293	       17	   858971	    14.66%	    16.75	    50.53
ipinyou, camp=3476, algo=mcpc, N=1000, c0=0.03125      	         36	   350000	      16254	       36	   865811	     4.64%	    53.27	    24.05
ipinyou, camp=3476, algo=lin_bid, N=1000, c0=0.03125   	        113	   350000	       7915	      113	   352671	     2.26%	    44.56	     3.12
ipinyou, camp=3476, algo=rlb, N=1000, c0=0.03125       	        113	   350000	      18282	      113	   855048	     5.22%	    46.77	     7.57
```
Note these results are produced from a subset (the first 350,000 lines of each campaign in iPinYou) under T = 1000 and c0 = 1/32.
For the full small-scale evaluation and large-scale evaluation, please first check the GitHub project [make-ipinyou-data](https://github.com/wnzhang/make-ipinyou-data "make-ipinyou-data") for pre-processing the [iPinYou data](http://data.computational-advertising.org "iPinYou data"). 
After downloading the dataset, by "make all" you can generate the standardised data.
