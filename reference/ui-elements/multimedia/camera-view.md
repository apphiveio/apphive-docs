---
description: Provides access to the local camera view or photo library.
---

# Camera View

![](../../../.gitbook/assets/captura-de-pantalla-2020-02-06-a-la-s-14.07.52.png)

### ⚙ Properties

* **Generic properties**
  * **Enable** [**skeleton loaders**](../../styles/skeleton-loader.md)**:** this tool provides an indication to the user that something is coming but not yet available on the camera view element.
  * **Control is hidden:** hide the camera view element from the screen.

{% hint style="info" %}
The [**skeleton loader**](../../styles/skeleton-loader.md) component provides a user with a visual indicator that content is coming/loading. This is better received than traditional full-screen loaders.
{% endhint %}

### 👆 Events

* **On QR code read:** implements a view which show camera and notify when there's a QR code inside the preview.
* **On take picture:** called when image data is available after a picture is taken.

