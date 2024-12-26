This repository contains a Dockerfile with a common error and its solution.  The original Dockerfile fails to start the application because the CMD instruction is improperly configured. The solution provides a corrected Dockerfile that successfully runs the application.

## Problem

The provided Dockerfile uses `CMD ["npm", "start"]`.  This works only if a start script is defined in package.json. If the application entry point requires a different command, the application may fail to run.