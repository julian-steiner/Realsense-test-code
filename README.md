<a name="readme-top"></a>
<h3 align="center">Realsense python test code</h3>

  <p align="center">
    This is a really simple project that shows how to use the camera and should serve as a starter.
  <p />

<!-- GETTING STARTED -->
### Prerequisites
- Python 3.11.4 was used

### Installation

1. Create a virtual environment and activate it
    ```sh
    python3 -m venv venv

    # Windows
    ./venv/scripts/activate

    # Linux
    source /venv/bin/activate
    ```
2. Install the dependencies
    ```sh
    pip3 install -r requirements.txt
    ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

This is a really simple example of just getting the camera to work. The depth and color image have the same format and are aligned by the camera itself. 

This means that you can easily get the depth of a point.
```python
# Some random point
point = color_image[y][x]

# To get the depth of this point
depth = depth_image[y][x] * depth_scale
```
You should be able to run some object or shape or april tag recognition on the color image and then get the depth with the depth image which would make the calculations really easy.

<p align="right">(<a href="#readme-top">back to top</a>)</p>