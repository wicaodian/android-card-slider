![Alt Text](https://github.com/wicaodian/android-card-slider/blob/main/demo.gif)



# CARDSLIDER [JAVA/Kotlin]
Material design UI controller that allows to swipe through cards with pictures and descriptions

credit to [original author](https://github.com/Ramotion/cardslider-android)

I just updated the library since they were not updating it anymore.
Converted their library to Kotlin Thanks to [armancodv](https://github.com/armancodv) for his pull-request


I've successfully updated our project to resolve previous Gradle build issues,
ensuring compatibility with the latest versions of Gradle and Kotlin.

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

## Future Support

Please note that while I'm committed to maintaining the project for now, I may not be able to provide long-term support. 
I encourage the community to step in and help keep the project alive and thriving. 
Your contributions and support can make a big difference!

If you're interested in taking a more active role in maintaining this project, please reach out. I'd love to hear from anyone willing to help.

Thank you for your interest and support!
