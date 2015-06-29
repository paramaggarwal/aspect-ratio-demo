# aspect-ratio-demo
A demo React Native app, to try out the new aspectRatioBox prop for views.

This demonstrates the changes in this PR: https://github.com/facebook/react-native/pull/1538

# Screenshot

![Screenshot of the running app](https://github.com/paramaggarwal/aspect-ratio-demo/raw/master/Screenshot.png)

# Run

1. Download the repo.
2. Open `AspectRatioDemo.xcodeproj`
3. Click `Run` in Xcode.

# Code

```
<View style={{width: viewWidth, backgroundColor: 'white'}}>
  <Image
    aspectRatioBox={{
      width: 612,
      height: 456,
    }}
    source={{
      uri: "http://edibleapple.com/wp-content/uploads/2009/11/steve-jobs-bill-gates-1991.jpg",
    }}
  />

  <View aspectRatioBox={{
    width: 1,
    height: 1,
  }} style={{alignSelf: 'stretch', flex: 1}}>
    <View style={{flexDirection: 'row', flex: 1}}>
      <Image
        style={{margin: 2, flex: 1}}
        source={{uri: "http://edibleapple.com/wp-content/uploads/2009/11/steve-jobs-bill-gates-1991.jpg"}}
      />
      <Image
        style={{margin: 2, flex: 2}}
        source={{uri: "http://edibleapple.com/wp-content/uploads/2009/11/steve-jobs-bill-gates-1991.jpg"}}
      />
    </View>
    <View style={{flexDirection: 'row', flex: 1}}>
      <Image
        style={{margin: 2, flex: 3}}
        source={{uri: "http://edibleapple.com/wp-content/uploads/2009/11/steve-jobs-bill-gates-1991.jpg"}}
      />
      <Image
        style={{margin: 2, flex: 2}}
        source={{uri: "http://edibleapple.com/wp-content/uploads/2009/11/steve-jobs-bill-gates-1991.jpg"}}
      />
    </View>
  </View>
</View>
```

# Author

Param Aggarwal (paramaggarwal@gmail.com)

# License

MIT
