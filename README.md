The built-in `UISegmentedControl` does not let you de-select elements.

This subclass allows it.

E.g.
```swift
    // in some class somewhere
    @IBOutlet weak var segmentControl: UISegmentedControl!
    @IBAction func segmentControlChanged(sender: UISegmentedControl) {
        // returns nil if the user just de-selected the selected segment by tapping on it
        sender.titleForSegmentAtIndex(sender.selectedSegmentIndex) 
    }
```
