This is a repo to replicate what I believe is a bug in Avalonia:
> Facing what looks like a bug with the pointer position in a `PointerWheelEventArgs`: it looks like the point computed from `e.GetCurrentPoint(control)` is 1 scroll step behind. It's not very visible when using a mousepad to scroll, but very very visible with a mouse

How to replicate the bug
1. Launch the app
2. Using a mouse, place the cursor in one of the buttons in the middle of the window
3. Without moving the mouse, scroll up or down. The highlighted button will be 2 steps above or below, which corresponds to 1 scroll step lag (scroll step is 50, button height is 25)
