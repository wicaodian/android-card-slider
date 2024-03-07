# CARDSLIDER [JAVA/Kotlin]
Material design UI controller that allows to swipe through cards with pictures and descriptions

credit to [original author](https://github.com/Ramotion/cardslider-android)

I just updated the library since they were not updating it anymore.
Converted their library to Kotlin Thanks to [armancodv](https://github.com/armancodv) for his pullrequest

I just fixed the old gradle build issues and make it working with the latest gradle and kotlin version.
together we can keep it improving

## Basic Usage
`CardSlider` is a custom `LayoutManager` for `RecyclerView`. You can attach it to RecyclerView from code or XML layout.

Here are the attributes you can specify in the constructor or XML layout:
- `activeCardLeft` - Active card offset from start of RecyclerView. Default value is 50dp.
- `cardWidth` - Card width. Default value is 148dp.
- `cardsGap` - Distance between cards. Default value is 12dp.

For card snapping, there is `CardSnapHelper` class.'
```Java
...
@Override
protected void onCreate(Bundle savedInstanceState) {
    ...
    recyclerView = (RecyclerView) findViewById(R.id.recycler_view);
    recyclerView.setLayoutManager(new CardSliderLayoutManager(this););

    new CardSnapHelper().attachToRecyclerView(recyclerView);
    ...
}
```

