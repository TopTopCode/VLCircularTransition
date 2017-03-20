# VLCircularTransition
Circular ViewController Transition

## Synopsis

VLCircularTransition gives you the leverage to customize Apple's boring viewcontroller animation to a smooth circular transition.

## Demo
[![vlcircularTransitionGif.gif](https://s16.postimg.org/paqqjdwlx/vlcircular_Transition_Gif.gif)](https://postimg.org/image/u9e8xx0ep/)

## Code Example
Declare & Initialize VLCircularTransition.

```
let transition = VLCircularTransition()

```
Set the required callback for presenting ViewController
```

    func animationController(forPresented presented: UIViewController, presenting: UIViewController, source: UIViewController) -> UIViewControllerAnimatedTransitioning? {
        transition.transitionMode = .present
        transition.startingPoint = self.facebookButton.center
        transition.circleColor = self.facebookButton.backgroundColor!
        
        return transition
        
    }
    
```
    
Set the required callback for dismissing ViewController

 ```
    func animationController(forDismissed dismissed: UIViewController) -> UIViewControllerAnimatedTransitioning? {
        
        transition.transitionMode = .dismiss
        transition.transitionMode = .dismiss
        transition.startingPoint = self.facebookButton.center
        transition.circleColor = self.facebookButton.backgroundColor!
        
        return transition
    }
  ```

## Requirements

iOS 9 or later.

## Contributors

- Vignesh Lakshminarayanan; Email: its.vigneshere@gmail.com

## Licence

The project was developed using Apple's Open-Source SDK making use of Swift Syntax. The code is free to use & download.  
