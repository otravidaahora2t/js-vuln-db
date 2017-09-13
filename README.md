# Case Study of JavaScript Engine Vulnerabilities

## V8

CVE Number | Feature | Keywords | Credit
---------- | ------- | -------- | ------
[CVE-2013-6632](./v8/CVE-2013-6632.md) | TypedArray | Integer Overflow, OOB | _Pinkie Pie_
[CVE-2014-1705](./v8/CVE-2014-1705.md) | TypedArray | Invalid Array Length, OOB | _geohot_
[CVE-2014-3176](./v8/CVE-2014-3176.md) | Array.concat | Side Effect, OOB | _lokihardt_
[CVE-2014-7927](./v8/CVE-2014-7927.md) | Optimization | asm.js, OOB | _Christian Holler_
[CVE-2014-7928](./v8/CVE-2014-7928.md) | Optimization | Array | _Christian Holler_
[CVE-2015-1233](./v8/CVE-2015-1233.md) | Optimization | Array, OOB | ?
[CVE-2015-1242](./v8/CVE-2015-1242.md) | Optimization | Array, Type Confusion | _fcole@onshape.com_
[CVE-2015-6764](./v8/CVE-2015-6764.md) | JSON.stringify | Side Effect, OOB, | _Guang Gong [[1]](#qihoo360)_
[CVE-2015-6771](./v8/CVE-2015-6771.md) | TypedArray.map | Prototype, OOB | ?
[CVE-2015-8584](./v8/CVE-2015-8548.md) | JSON.stringify | Side Effect, OOB | ?
[CVE-2016-1646](./v8/CVE-2016-1646.md) | Array.concat | Side Effect, OOB | _Wen Xu [[2]](#keenlab)_
[CVE-2016-1653](./v8/CVE-2016-1653.md) | Optimization | asm.js, TypedArray, OOB | _Choongwoo Han [[6]](#kaistsoftsec)_
[CVE-2016-1665](./v8/CVE-2016-1665.md) | Optimization | asm.js | _HyungSeok Han [[6]](#kaistsoftsec)_
[CVE-2016-1669](./v8/CVE-2016-1669.md) | RegExp | Heap Overflow, Integer Overflow | _Choongwoo Han [[6]](#kaistsoftsec)_
[CVE-2016-1677](./v8/CVE-2016-1677.md) | decodeURI | Side Effect, Information Leak | _Guang Gong [[1]](#qihoo360)_
[CVE-2016-1688](./v8/CVE-2016-1688.md) | RegExp | | _Max Korenko_
[CVE-2016-5129](./v8/CVE-2016-5129.md) | Array | Side Effect | _Jeonghoon Shin_
[CVE-2016-5172](./v8/CVE-2016-5172.md) | | Scope | _Choongwoo Han [[6]](#kaistsoftsec)_
[CVE-2016-5198](./v8/CVE-2016-5198.md) | Optimization | parseInt, Compiler, OOB | _Tencent Keen Security Lab_
[CVE-2016-5200](./v8/CVE-2016-5200.md) | Optimization | asm.js TypedArray, OOB | _Choongwoo Han [[6]](#kaistsoftsec)_
[CVE-2016-9651](./v8/CVE-2016-9651.md) | Object.assign | Logic, Property | _Guang Gong [[1]](#qihoo360)_
[CVE-2017-5030](./v8/CVE-2017-5030.md) | Array.concat | Side Effect, OOB | _Brendon Tiszka_
[CVE-2017-5040](./v8/CVE-2017-5040.md) | Array.indexOf | TypedArray, Side Effect, Buffer Neutering | _Choongwoo Han_
[CVE-2017-5053](./v8/CVE-2017-5053.md) | Array.indexOf | Side Effect | _Team Sniper [[2]](#keenlab)_
[CVE-2017-5070](./v8/CVE-2017-5070.md) | Optimization | Array, Type Confusion | _Zhao Qixun [[5]](#qihoo360vulcan)_
[CVE-2017-5071](./v8/CVE-2017-5071.md) | Compiler | OOB | _Choongwoo Han_

## ChakraCore
CVE Number | Feature | Keywords | Credit
---------- | ------- | -------- | ------
[CVE-2016-3386](./chakra/CVE-2016-3386.md) | Spread Operator | Array, Proxy, Stack Overflow | _Richard Zhu_
[CVE-2016-7189](./chakra/CVE-2016-7189.md) | Array.join | Information Leak | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7190](./chakra/CVE-2016-7190.md) | Array.map | Heap Overflow | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7194](./chakra/CVE-2016-7194.md) | Function.apply | Information Leak | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7200](./chakra/CVE-2016-7200.md) | Array.filter | Heap Corruption | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7201](./chakra/CVE-2016-7201.md) | Array | Prototype, Type Confusion | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7202](./chakra/CVE-2016-7202.md) | Array.reverse | Overflow | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7203](./chakra/CVE-2016-7203.md) | Array.splice | Heap Overflow | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7240](./chakra/CVE-2016-7240.md) | eval | Proxy, Type Confusion | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7241](./chakra/CVE-2016-7241.md) | JSON.parse | Information Leak | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7286](./chakra/CVE-2016-7286.md) | SIMD.toLocaleString | Uninitialized Memory | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7287](./chakra/CVE-2016-7287.md) | Intl | Initialization, Type Confusion | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2016-7288](./chakra/CVE-2016-7288.md) | TypedArray.sort | Side Effect, Buffer Neutering | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2017-0015](./chakra/CVE-2017-0015.md) | Spread Operator | Side Effect, Uninitialized Memory | _Qixun Zhao [[4]](#qihoo360skyeye)_<br/> _lokihart_<br/> _Simon Zuckerbraun_
[CVE-2017-0071](./chakra/CVE-2017-0071.md) | Optimization | Array, Type Confusion | _lokihardt [[3]](#projectzero)_
[CVE-2017-0134](./chakra/CVE-2017-0134.md) | Array.concat | Side Effect, Type Confusion | _Jordan Rabet_
[CVE-2017-0141](./chakra/CVE-2017-0141.md) | Array.reverse | Side Effect | _Semmle Inc_
[CVE-2017-8548](./chakra/CVE-2017-8548.md) | Optimization | Array | _lokihardt [[3]](#projectzero)_
[CVE-2017-8601](./chakra/CVE-2017-8601.md) | Optimization | Array | _lokihardt [[3]](#projectzero)_
[CVE-2017-8634](./chakra/CVE-2017-8634.md) | Array.concat | Side Effect | _Hao Lian [[5]](#qihoo360vulcan)_<br/>_HyungSeok Han [[6]](#kaistsoftsec)_
[CVE-2017-8636](./chakra/CVE-2017-8636.md) | Compiler | Integer Overflow | _lokihardt [[3]](#projectzero)_
[CVE-2017-8640](./chakra/CVE-2017-8640.md) | arguments, | Compiler, Uninitialize Memory | _lokihardt [[3]](#projectzero)_
[CVE-2017-8645](./chakra/CVE-2017-8645.md) | Compiler | asm.js | _lokihardt [[3]](#projectzero)_
[CVE-2017-8646](./chakra/CVE-2017-8646.md) | Compiler | asm.js | _lokihardt [[3]](#projectzero)_
[CVE-2017-8656](./chakra/CVE-2017-8656.md) | try | Uninitialized Memory | _lokihardt [[3]](#projectzero)_
[CVE-2017-8657](./chakra/CVE-2017-8657.md) | Compiler | asm.js | _lokihardt [[3]](#projectzero)_
[CVE-2017-8670](./chakra/CVE-2017-8670.md) | arguments | Compiler, Uninitialize Memory | _lokihardt [[3]](#projectzero)_
[CVE-2017-8671](./chakra/CVE-2017-8671.md) | Function.call | Integer Overflow | _lokihardt [[3]](#projectzero)_

## JavaScriptCore
CVE Number | Feature | Keywords | Credit
---------- | ------- | -------- | ------
[CVE-2016-1857](./jsc/CVE-2016-1857.md) | Array.join | Side Effect, Use After Free | _Liang Chen_, _Zhen Feng_, _wushi_ _[[2]](#keenlab)_<br/> _Jeonghoon Shin_
[CVE-2016-4622](./jsc/CVE-2016-4622.md) | Array.slice | Side Effect, OOB | _Samuel Groß_
[CVE-2016-4734](./jsc/CVE-2016-4734.md) | TypedArray.copyWithin<br/> TypedArray.fill | Side Effect, Buffer Neutering | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2017-2446](./jsc/CVE-2017-2446.md) | Funciton.caller | Type Confusion | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2017-2447](./jsc/CVE-2017-2447.md) | Function.bind | OOB | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2017-2464](./jsc/CVE-2017-2464.md) | Array.concat | Integer Overflow | _Natalie Silvanovich [[3]](#projectzero)_
[CVE-2017-2491](./jsc/CVE-2017-2491.md) | String.replace | RegExp, Use After Free | _Samuel Groß_, and _Niklas Baumstark_
[CVE-2017-2521](./jsc/CVE-2017-2521.md) | Array.length | OOB | _lokihardt [[3]](#projectzero)_
[CVE-2017-2531](./jsc/CVE-2017-2531.md) |  | OOB | _lokihardt [[3]](#projectzero)_
[CVE-2017-2536](./jsc/CVE-2017-2536.md) | Spread Operator | Array, Integer Overflow | _Samuel Groß_, and _Niklas Baumstark_
[CVE-2017-2547](./jsc/CVE-2017-2547.md) | Optimization | parseInt, Compiler, OOB | _lokihardt [[3]](#projectzero)_
[CVE-2017-6980](./jsc/CVE-2017-6980.md) | Array.splice | Uninitialized Memory | _lokihardt [[3]](#projectzero)_
[CVE-2017-6984](./jsc/CVE-2017-6984.md) | Intl.getCanonicalLocales | Heap Overflow | _lokihardt [[3]](#projectzero)_
[CVE-2017-7056](./jsc/CVE-2017-7056.md) | arguments | Uninitialized Memory | _lokihardt [[3]](#projectzero)_
[CVE-2017-7061](./jsc/CVE-2017-7061.md) | Compiler | Array, Type Confusion | _lokihardt [[3]](#projectzero)_

## SpiderMonkey
CVE Number | Feature | Keywords | Credit
---------- | ------- | -------- | ------
[CVE-2014-1513](./spidermonkey/CVE-2014-1513.md) | TypedArray.subarray | OOB, Buffer Neutering, Side Effect | _Jüri Aedla_

---
<a name="qihoo360"></a>[1] Qihoo 360  
<a name="keenlab"></a>[2] Tencent KeenLab  
<a name="projectzero"></a>[3] Google Project Zero  
<a name="qihoo360skyeye"></a>[4] Qihoo 360 Skyeye Labs  
<a name="qihoo360vulcan"></a>[5] Qihoo 360 Vulcan Team  
<a name="kaistsoftsec"></a>[6] KAIST SoftSec  
