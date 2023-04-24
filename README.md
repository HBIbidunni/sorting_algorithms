# The ALX Project Sorting algorithms & Big O
---------
In this project, the core learnings center on `sorting algorithms` and the `Big O`:

* Where <b>sorting algorithms</b> are used to arrange a collection of elements in a particular order
* Then the <b>Big O notation</b> is used to describe the upper bound of an algorithm's time complexity, which is how the algorithm's performance scales as the size of the input data increases.
* One important consideration when choosing a <b>sorting algorithm</b> is its efficiency, which is often expressed using the <b>Big O</b> notation.
* There are many <b>sorting algorithms</b>, each with its own advantages and disadvantages, but they all aim to accomplish the same goal. 
* <b>Sorting algorithms</b> are commonly used in computer science and programming to manage large datasets, search and compare values, and analyze data. 

## Project Requirements :bulb:
* All files will be compiled on <b>Ubuntu 20.04 LTS</b> using <b>gcc</b>, using the options <b>-Wall -Werror -Wextra -pedantic -std=gnu89</b>.
* This is a `C` project, hence all codes should use the `Betty` style.
* All files should end with a new line.
* The project should contain :two: helper files: <b>print_array.c</b>,  a `C` function that prints an array of integers and <b>print_list.c</b>,  a `C` function that prints a `listint_t` doubly-linked list.
* The prototypes of all functions should be included in your header file called `sort.h` and should be include guarded.

## Header file :file_folder:
The header file [sort.h](./sort.h) has the following data structure:

```
typedef struct listint_s
{
	const int n;
	struct listint_s *prev;
	struct listint_s *next;
} listint_t;
```
## Tests :white_check_mark:
* [tests](./tests): This contains all the test files of the project.

## Function Prototypes :white_check_mark:

| File                       | Prototype                                         |
| -------------------------- | ------------------------------------------------- |
| `print_array.c`            | `void print_array(const int *array, size_t size)` |
| `print_list.c`             | `void print_list(const listint_t *list)`          |
| `0-bubble_sort.c`          | `void bubble_sort(int *array, size_t size);`      |
| `1-insertion_sort_list.c`  | `void insertion_sort_list(listint_t **list);`     |
| `2-selection-sort.c`       | `void selection_sort(int *array, size_t size);`   |
| `3-quick_sort.c`           | `void quick_sort(int *array, size_t size);`       |
| `100-shell_sort.c`         | `void shell_sort(int *array, size_t size);`       |
| `101-cocktail_sort_list.c` | `void cocktail_sort_list(listint_t **list);`      |
| `102-counting_sort.c`      | `void counting_sort(int *array, size_t size);`    |
| `103-merge_sort.c`         | `void merge_sort(int *array, size_t size);`       |
| `104-heap_sort.c`          | `void heap_sort(int *array, size_t size);`        |
| `105-radix_sort.c`         | `void radix_sort(int *array, size_t size);`       |
| `106-bitonic_sort.c`       | `void bitonic_sort(int *array, size_t size);`     |
| `107-quick_sort_hoare.c`   | `void quick_sort_hoare(int *array, size_t size);` |

* [deck.h](./deck.h): Header file containing definitions and prototypes for all types and functions written for the task `1000-sort_deck.c`.

<b>Data Structures</b>:
```
typedef enum kind_e
{
	SPADE = 0,
	HEART,
	CLUB,
	DIAMOND
} kind_t;

typedef struct card_s
{
	const char *value;
	const kind_t kind;
} card_t;

typedef struct deck_node_s
{
	const card_t *card;
	struct deck_node_s *prev;
	struct deck_node_s *next;
} deck_node_t;
```

<b>Function Prototype</b>:

| File               | Prototype                             |
| ------------------ | ------------------------------------- |
| `1000-deck_node.c` | `void sort_deck(deck_node_t **deck);` |


> All comments, feedbacks and suggestions are highly welcome. Kindly take a look at my codes to get an insight. Scroll up :arrow_up:, please.


##  Author :black_nib:
*  __Oyindamola Ibis__ <[HBIbidunni](https://github.com/HBIbidunni)>
-------
