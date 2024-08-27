# Exam_1

# Multilevel-doubly-linked-list
my_project/
│
├── CMakeLists.txt
├── src/
│   ├── node.c
│   └── node.h
├── tests/
│   ├── main_test.cpp
│   └── document.txt
└── build/


#build:
sudo apt-get install libgtest-dev

cd /usr/src/gtest
sudo cmake .
sudo make
sudo cp libgtest*.a /usr/lib

mkdir build
cd build
cmake ..

make

./test_runner

make clean

valgrind --leak-check=full --show-leak-kinds=all ./test_runner

gdb ./test_runner
