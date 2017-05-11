The parameters used and times of your slowest
```
Mapper Containers=8
Reducer Containers=1
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

teragen
real	1m17.648s
user	0m6.537s
sys	0m0.787s

terasort
real	3m48.141s
user	0m8.703s
sys	0m0.857s
Deleted /results/tg-10GB-8-1-512
Deleted /results/ts-10GB-8-1-512
```
The parameters used and times of your fastest 
```
Mapper Containers=2
Reducer Containers=4
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

teragen
real	1m13.875s
user	0m5.665s
sys	0m0.738s

terasort
real	3m17.541s
user	0m8.776s
sys	0m0.973s
Deleted /results/tg-10GB-2-4-1024
Deleted /results/ts-10GB-2-4-1024
```

```
[hdfs@ip-172-31-27-157 tmp]$ ./YARNtest.sh 
Testing loop started on Tue May 9 09:59:06 UTC 2017
Mapper Containers=2
Reducer Containers=1
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m18.619s
user	0m6.206s
sys	0m0.771s

real	3m48.780s
user	0m9.516s
sys	0m0.922s
Deleted /results/tg-10GB-2-1-512
Deleted /results/ts-10GB-2-1-512
Mapper Containers=2
Reducer Containers=1
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m17.028s
user	0m5.977s
sys	0m0.696s

real	3m40.477s
user	0m7.853s
sys	0m0.837s
Deleted /results/tg-10GB-2-1-1024
Deleted /results/ts-10GB-2-1-1024
Mapper Containers=2
Reducer Containers=2
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m17.332s
user	0m5.821s
sys	0m0.763s

real	3m17.715s
user	0m8.472s
sys	0m0.803s
Deleted /results/tg-10GB-2-2-512
Deleted /results/ts-10GB-2-2-512
Mapper Containers=2
Reducer Containers=2
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m19.497s
user	0m6.160s
sys	0m0.621s

real	3m21.350s
user	0m8.440s
sys	0m0.814s
Deleted /results/tg-10GB-2-2-1024
Deleted /results/ts-10GB-2-2-1024
Mapper Containers=2
Reducer Containers=4
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m23.501s
user	0m5.919s
sys	0m0.732s

real	3m33.116s
user	0m8.251s
sys	0m0.924s
Deleted /results/tg-10GB-2-4-512
Deleted /results/ts-10GB-2-4-512
Mapper Containers=2
Reducer Containers=4
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m13.875s
user	0m5.665s
sys	0m0.738s

real	3m17.541s
user	0m8.776s
sys	0m0.973s
Deleted /results/tg-10GB-2-4-1024
Deleted /results/ts-10GB-2-4-1024
Mapper Containers=4
Reducer Containers=1
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m24.132s
user	0m5.987s
sys	0m0.761s

real	3m42.379s
user	0m8.608s
sys	0m0.914s
Deleted /results/tg-10GB-4-1-512
Deleted /results/ts-10GB-4-1-512
Mapper Containers=4
Reducer Containers=1
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m15.937s
user	0m6.134s
sys	0m0.727s

real	3m43.391s
user	0m8.221s
sys	0m0.902s
Deleted /results/tg-10GB-4-1-1024
Deleted /results/ts-10GB-4-1-1024
Mapper Containers=4
Reducer Containers=2
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m15.577s
user	0m6.167s
sys	0m0.718s

real	3m29.815s
user	0m8.446s
sys	0m0.853s
Deleted /results/tg-10GB-4-2-512
Deleted /results/ts-10GB-4-2-512
Mapper Containers=4
Reducer Containers=2
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m21.279s
user	0m6.254s
sys	0m0.792s

real	3m23.727s
user	0m8.709s
sys	0m0.898s
Deleted /results/tg-10GB-4-2-1024
Deleted /results/ts-10GB-4-2-1024
Mapper Containers=4
Reducer Containers=4
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m16.549s
user	0m5.773s
sys	0m0.795s

real	3m33.138s
user	0m8.134s
sys	0m0.832s
Deleted /results/tg-10GB-4-4-512
Deleted /results/ts-10GB-4-4-512
Mapper Containers=4
Reducer Containers=4
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m16.914s
user	0m5.798s
sys	0m0.775s

real	3m29.191s
user	0m7.957s
sys	0m0.933s
Deleted /results/tg-10GB-4-4-1024
Deleted /results/ts-10GB-4-4-1024
Mapper Containers=8
Reducer Containers=1
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m17.648s
user	0m6.537s
sys	0m0.787s

real	3m48.141s
user	0m8.703s
sys	0m0.857s
Deleted /results/tg-10GB-8-1-512
Deleted /results/ts-10GB-8-1-512
Mapper Containers=8
Reducer Containers=1
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m23.215s
user	0m5.929s
sys	0m0.709s

real	3m50.567s
user	0m8.175s
sys	0m0.813s
Deleted /results/tg-10GB-8-1-1024
Deleted /results/ts-10GB-8-1-1024
Mapper Containers=8
Reducer Containers=2
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m18.662s
user	0m6.625s
sys	0m0.868s

real	3m27.535s
user	0m8.502s
sys	0m0.845s
Deleted /results/tg-10GB-8-2-512
Deleted /results/ts-10GB-8-2-512
Mapper Containers=8
Reducer Containers=2
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m20.882s
user	0m6.123s
sys	0m0.773s

real	3m31.676s
user	0m8.985s
sys	0m0.885s
Deleted /results/tg-10GB-8-2-1024
Deleted /results/ts-10GB-8-2-1024
Mapper Containers=8
Reducer Containers=4
Container Memory=512 MB
Mapper JVM Heap=409 MB
Reducer JVM Heap=409 MB

real	1m21.115s
user	0m6.038s
sys	0m0.821s

real	3m41.292s
user	0m8.476s
sys	0m0.922s
Deleted /results/tg-10GB-8-4-512
Deleted /results/ts-10GB-8-4-512
Mapper Containers=8
Reducer Containers=4
Container Memory=1024 MB
Mapper JVM Heap=819 MB
Reducer JVM Heap=819 MB

real	1m12.482s
user	0m5.822s
sys	0m0.713s

real	3m29.756s
user	0m8.448s
sys	0m0.897s
Deleted /results/tg-10GB-8-4-1024
Deleted /results/ts-10GB-8-4-1024
Testing loop ended on Thu May 11 08:28:42 UTC 2017
```
