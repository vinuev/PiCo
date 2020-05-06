# PiCo
cd PiCo/
mkdir fastflow
cd fastflow/
git clone  https://github.com/fastflow/fastflow.git /Users/vinu.venugopal/Documents/ULProjects/PiCo/fastflow


cd pico
ln -s ../fastflow/ff .


/Users/vinu.venugopal/Documents/ULProjects/PiCo/pico/examples/stock-market

g++ -o stock_pricing_stream -I/Users/vinu.venugopal/Documents/ULProjects/PiCo/pico/include -I/Users/vinu.venugopal/Documents/ULProjects/PiCo/pico -std=c++11 stock_pricing_stream.cpp


cat testdata/stock_options_64K.txt | nc -l 4000 && ./a.out localhost 4000

cat testdata/stock_options_64K.txt | nc -l 4000 && ./stock_pricing_stream localhost 4000

cd testdata/

-------------

g++ -o stock_tweets -I/Users/vinu.venugopal/Documents/ULProjects/PiCo/pico/include -I/Users/vinu.venugopal/Documents/ULProjects/PiCo/pico -std=c++11 stock_tweets.cpp
 
