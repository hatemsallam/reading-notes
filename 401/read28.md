# Create dynamic lists with RecyclerView

* There are Several different classes work together to build dynamic list:
  * RecyclerView : is the ViewGroup that contains the views corresponding to your data,you add RecyclerView into your layout .
  * view holder object: Each individual element in the list is defined by it .
  * The RecyclerView requests those views, and binds the views to their data, by calling methods in the adapter. You define the adapter by extending RecyclerView.Adapter.
  * The layout manager arranges the individual elements in your list.

## Steps for implementing RecyclerView

1. decide what the list or grid is going to look like.
2. Design how each element in the list is going to look and behave.
3. Define the Adapter that associates your data with the ViewHolder views.

## Plan your layout

* The RecyclerView library provides three layout managers : 

1. LinearLayoutManager :arranges the items in a one-dimensional list.
2. GridLayoutManager arranges all items in a two-dimensional grid.
3. StaggeredGridLayoutManager is similar to GridLayoutManager, but it does not require that items in a row have the same height (for vertical grids) or items in the same column have the same width (for horizontal grids).

## Implementing adapter and view holder

* The ViewHolder is a wrapper around a View that contains the layout for an individual item in the list.
* When we define our adapter, we need to override three key methods:
    1. onCreateViewHolder()
    2. onBindViewHolder()
    3. getItemCount()