# How to add an entry?

- Create a folder in format `DD-MM-YYYY` in _\_includes_ folder
- Create `index.md` in this folder and put your content there
- If the entry contains images, create another `DD-MM-YYYY` folder in `assets/images` folder and put your media in it

  - Name the images in the following format `i_X.png` where X the count of image being added
  - Reference the image from `index.md` file like this:
    ```
    ![Alt Text](assets/images/DD-MM-YY/iX.png)
    ```
  - To display it in VS Code preview, add `/` to the beginning of path. That is
    ```
    ![Alt Text](/assets/images/DD-MM-YY/iX.png)
    ```

- Add the following to the project level _index.md_ file:
  ```
  {% include DD-MM-YYYY/index.md %}
  ```

# How to deploy?

Just push to `main` branch. CI/CD will automatically deploy!
