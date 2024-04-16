# important points to be noted !

## Wayland doesn't know how to create buffers, nor how to draw into them. That's the responsibility of other drawing packages, such as OpenGL.

In principle, any system capable of creating buffers and drawing into them should be usable. At present, Wayland only supports a system called EGL. It does so by the four functions

wl_egl_window_create
wl_egl_window_destroy
wl_egl_window_resize
wl_egl_window_get_attached_size
