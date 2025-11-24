# CTF Challenge

## Setup
1. Install Docker and cmgr
2. Set environment variables:
```bash
   export CMGR_DB=~/cmgr/cmgr.db
   export CMGR_ARTIFACTS_DIR=~/cmgr/artifacts
   export DOCKER_API_VERSION=1.41
```
3. Configure Docker daemon (`/etc/docker/daemon.json`):
```json
   {
     "min-api-version": "1.41"
   }
```
4. Restart Docker: `sudo service docker restart`

## Run Challenge
```bash
cd challenges/my-forensics
cmgr update
cmgr playtest 18739/stop-the-exfil
```

Access at: http://localhost:4242/

## Challenge Details
- **Namespace**: 18739
- **Category**: Forensics
