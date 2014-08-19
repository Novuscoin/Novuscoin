Novuscoin integration/staging tree
================================

http://www.Novuscoin.org

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2013 Litecoin Developers
Copyright (c) 2014 Novuscoin Developers

What is Novuscoin?
----------------

Novuscoin is a light version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 1 minute per block
 - About 1440 blocks per day
 - We will premine about 150 billion in restricted Novuscoin mostly kept offline to be able to have reserves for lost or stolen coins, to use for the Zero interest loan program for NovuscoinRealty.com and NovuscoinCars.com
 - We will restrict the use and sale of the reserves so as to not disrupt market prices of Novuscoin. We want to ensure that we continue to maintain a stable price level.
 - The advantage of reserves are that if coins are lost or stolen we can easily reset the wallets and render stolen coins useless and locate all addresses prior to the theft and replace lost or stolen coins for the public. 
 - We estimate to have in circulation 236,471,000 coins by end of 2016
 - We have incremental payouts depending on difficulty. 
 - Finally to the minimum of 25 coins per block after 400,000 blocks.
 - 2016 blocks to retarget difficulty

License
-------

Novuscoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------
We need help with making the code better. If you are a developer we are paying a bounty for your help. Please contact us at webmaster@novuscoincorp.com.

"Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Novuscoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial."

The `master .08` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/Novuscoin/Novuscoin) are created
regularly to indicate new official, stable release versions of Novuscoin.

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

    qmake BITCOIN_QT_TEST=1 -o Makefile.test novuscoin-qt.pro
    make -f Makefile.test
    ./Novuscoin-qt_test

