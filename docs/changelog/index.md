# Changelog

## VisionAI Changelog

### **0.1.15** <small>February 7, 2023</small>

- 🐛 On linux we were using incorrect nvidia_smi package.
- 🎨 Add support for common spelling errors during commands (like scenarios instead of scenario)
- 🚚 Move scenario.json file to this repo - so everything is in one place.



### **0.1.14** <small>February 3, 2023</small>

- ✨ Support for `visionai scenario test` command.
- ✨ Support for Triton server running on MacOS (tested)
- 🔥 Simplified scenario command names (don't have to specify --name anymore)
- 📝 Renamed all cli files to _app - to avoid confusion between models.py & models/ module.
- 📝 Move add-scenario and remove-scenario to camera module (these are camera operations.)
- 🔥 Show nice progress bar while any docker image is being pulled.
- 🧪 Added results.show() method to detection that uses cv2.imshow() to show the results locally.

### **0.1.12** <small>January 31, 2023</small>

- ✨ Support for managing triton server
- 🎨 Start/stop triton server from CLI.
- 📝 Get/print models status coming from triton.
- 🔥 Implemented pretty printing through rich library for models
- 🧪 CI Tests to test both before & after package creation
- 🐛 Fix versioning bug (that broke the previous version)

### **0.1.11** <small>January 27, 2023</small>

- Support for Triton models (through http/grpc)
- Implemented yolov5 backend for triton
- Implemented Autoshape wrapper for NMS & scaling
- Added easy test case for reproducing.
- Updated schema for models, fix test cases for it.

### **0.1.10** <small>January 25, 2023</small>

- Implemented download models for scenarios
- Added cv2, torch, numpy dependencies for inference
- Added support for `--version` & `--verbose` options to cli
- CLI Test cases to use `python -m visionai` to replicate user behavior

### **0.1.7** <small>January 24, 2023</small>

- Implemented scenarios functionality
- Docker compose integration
- Makefile integration

### **0.1.7** <small>January 22, 2023</small>

- Implemented camera add/delete functionality

### **0.1.6** <small>January 20, 2023</small>

- Implemented initial set of commands in different files (dummy implementation)
- Testing commands individually or through the main application

### **0.1.3** <small>January 16, 2023</small>

- Basic overview and usage documentation is updated.
- Started using a termy JS script to show terminal animations nicely

### **0.1.2** <small>January 14, 20123</small>

- Made MkDocs documents based on Typer format
- Registered CNAME to point to [https://docs.visionify.ai](https://docs.visionify.ai)

### **0.1.1** <small>January 11, 2023</small>

- Updated Azure DevOps CI/CD to automatically publish package on each merge
- Initial set of commands for visionai application
- Made `visionai` as a callable CLI application through poetry

### **0.1.0** <small>January 10, 2023</small>

- Initial release: `pip install visionai`
- Pushed package to `PyPI` repository
