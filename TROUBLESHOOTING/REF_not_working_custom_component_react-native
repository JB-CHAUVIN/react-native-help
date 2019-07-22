## My ref is not working on a react native component  

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
