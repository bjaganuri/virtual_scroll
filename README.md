Logical steps used in implementing Virtual scroll are as bello:

1) Create an initial page with default records(say pageNO=1 with 10 records out of 10000) with some height(say 500px)
2) Attach onScroll event to the page created above in order to load next set of records once user scrolls
	2.1) onscroll get the offset height of scroll bar from top edge of the element to which scroll event has been attached
	2.2) If the scroll offeset height is more than the total height required show the data - height of the containing element 
     	 	increament the page number and load corresponding records
	3.3) Now total height required to show elements is pageno * height required by each element
