UGI
===
#ifndef HEAP
#define HEAP

#include <iostream>

using namespace std;

typedef int heapElement;


class Heap
{
	private:
		heapElement *myArray;
		int capacity;
		int size;

	public:
		Heap(int numOfElements = 26);
		Heap(const Heap& object2);
		bool isEmpty();
		void Insert(const heapElement& value);
		heapElement findMax();
		void deleteMax();
		void percolate_down();
		void percolate_up();
};

#endif
