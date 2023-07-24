<?php
$r = 0;
for ($i = 0; $i < 10000; $i++) {
    for ($j = 0; $j < 10000; $j++) {
coding=utf-8
s = raw_input()
punct = ".,?!:\"-';"
k = ''
for i in range(len(s)):
bad = False
for j in range(len(punct)):
    if (punct[j] == s[i]):
    bad = True
if not bad:
    k = k + s[i]
else:
    k = k + ' '     
if (s.count(' PHP ') > s.count(' JavaScript ')):
    print('PHP')
elif (s.count(' PHP ') > s.count(' JavaScript ')):
    print('JavaScript')
else:
    print('C++ or Java or Python.')
    
