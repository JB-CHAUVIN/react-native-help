## My ref is not working on a react native component  

# With redux

It can be because of REDUX... since it's a higher level wrapper ref are not passed to our child.
Make sur not to have REDUX, or say REDUX to use forwardRef :

Usage example :

```
export default compose(
  connect(
    mapStateToProps,
    mapDispatchToProps,
    null,
    { forwardRef: true },
  ),
)(CardForm);
```

# Without redux
Export your custom component the following way :

```
export default React.forwardRef((props, ref) => <HeaderSearchBar innerRef={ref} {...props} />);

```

And make sur to add the ref :

```  
render() {
    const { innerRef } = this.props;

    return (
      <View style={styles.container}>
        <SearchBar
          ref={innerRef}
        />
      </View>
    );
  }

```
