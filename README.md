# CoinBev.ai
CoinBev.ai is a Jekyll-based website built for the crypto beer revolution. It uses the Minimal Mistakes theme (dark skin) and is auto-deployed to GitLab Pages via a CI/CD pipeline.

It is made by the community with the goal to provide all important information about the project.

## Getting Started

### Prerequisites
- Ruby (>= 2.5)
- Bundler (`gem install bundler`)
- Jekyll (`gem install jekyll`)

### Installation
Don't worry, you do not need to touch any ruby code! Thats just the static page generator. If you know Markdown, CSS and HTML, you are perfect!

1. Clone the repository:
   ```
   git clone https://gitlab.com/yourusername/coinbev.ai.git
   cd coinbev.ai
   ```
2. Configure Bundler to use local directory (recommended):
   ```bundle config set --local path 'vendor/bundle'```

   This keeps all dependencies in the project's `vendor` directory instead of installing globally.
   Both `vendor/` and `.bundle/` are gitignored.
2. Install dependencies:
   ```bundle install```
3. Start the local server:
   ```bundle exec jekyll serve```
   Then open your browser at [http://localhost:4000](http://localhost:4000).

   Note: Always run `bundle exec jekyll clean` when:
   - You've modified `_config.yml`
   - You're experiencing caching issues
   - Site updates aren't showing up as expected
   - You want to ensure a fresh build

## Deployment

The site automatically deploys to GitHub Pages when changes are pushed to the main branch. The deployment process:

1. Builds the Jekyll site in a clean environment
2. Uploads the built site as an artifact
3. Deploys to GitHub Pages

The live site is available at: https://coinbevai.github.io/

## How to Contribute

There are 3 ways you can contribute:

1. **Fork & Pull Requests**  
   Fork the repository, make your changes, and submit a pull request to fix issues or improve the project.

2. **Issues**  
   For non-technical contributions or suggestions (like text/content improvements), open an issue with a detailed description of the problem or idea.

3. **Design Contributions**  
   Create image or video assets that can be used to improve the website’s look and feel. Submit these assets via a pull request or link them in an issue.

## Project Structure
- `_pages`: All content pages
 `_sass/minimal-mistakes/_custom.scss`: our custom css on top of the mmistakes/minimal-mistakes default theme.
- `_config.yml`: Project configuration including theme, plugins, and site settings.
- `_data/navigation.yml`: Contains navigation menu details.
- `_includes/footer.html`: Custom footer with social links and GitHub improvement prompt.
- `index.md`: Homepage.
- `README.md`: This file.

## Additional Information

- The site is built with a focus on community and transparency.
- Follow general code and contribution guidelines when submitting pull requests.
- For any questions or support, feel free to open an issue.

## License

### Community Project License (CPL) v1.0

Copyright (c) 2025 CoinBevAi

Permission is hereby granted, free of charge, to any person obtaining a copy of this Software and associated documentation files (the "Software"),
to use, reproduce, display, and modify the Software solely for participation in the CoinBev.ai community project,
subject to the following conditions:

1. The Software may not be redistributed, mirrored, or hosted on any domains or platforms that are not officially affiliated with the CoinBev.ai
   community project.
2. Any redistribution or derivative works must include this license text in its entirety.
3. Commercial use of the Software or images outside the scope of the CoinBev.ai community project is not permitted without prior written consent.
4. All modifications must clearly acknowledge the original source.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
