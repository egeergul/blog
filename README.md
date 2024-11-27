# How to add an entry?

- Create a folder in format `DD-MM-YYYY` in _\_includes_ folder
- Create `index.md` in this folder and put your content there
- If the entry contains images, create an `images` folder and put your media in it
  - Name the images in the following fomrat `i_X.png` where X the count of image being added
- Add the following to the project level _index.md_ file:
  ```
  {% include DD-MM-YYYY/index.md %}
  ```

# How to deploy?

Just push to `main` branch. CI/CD will automatically deploy!
