ANDES COIN
===========



What is AndesCoin?
----------------

AndesCoin is a cryptocurrency with the following specifications  
  
Algorithm 	Scrypt  
Type 	PoW  
Coin abbreviation 	ANDES  
Address letter 	A  
RPC port 	36434  
P2P port 	36433  
Block reward 	60 coins  
Block halving 	250000 blocks  
Coin supply 	33333333 coins  
Premine amount 	3333333 coins  
  
For more information, see https://andes-coin.com  
  
License  
-------

AndesCoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.  

Development process  
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the AndesCoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/andescoin/andescoin/tags) are created
regularly to indicate new official, stable release versions of AndesCoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./andescoin-qt_test


Installation
------------

>git clone https://github.com/andescoin andes  
>cd andes/src/leveldb  
	>chmod +x build_detect_platform  
	>make clean  
	>make libleveldb.a libmemenv.a  
	>cd..  
	>mkdir obj  
	>make -f makefile.unix  
	>./andescoind  


**Copyright (c) 2018 AndesCoin Developers**


