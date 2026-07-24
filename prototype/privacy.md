# Privacy and consent

## Purpose
Define privacy and consent requirements for the Starlight prototype.

## Principles
- explicit consent for capture and processing
- minimal data sharing across devices
- user control over what is synced and stored
- transparency about how captured content is used

## Capture consent
- ask the user before processing any audio, image, or command capture
- show what will be sent to AI and storage
- allow the user to cancel before processing begins

## Device sharing
- glasses should only send approved capture items to the phone
- phone should only sync approved items to the cloud and laptop
- keep unwanted content local and private

## Sync and storage
- store only the selected task/context state needed for continuity
- encrypt sync payloads in transit
- avoid storing raw audio or image data unless explicitly authorized

## Revocation
- allow users to revoke sharing for individual items
- provide a simple way to delete synced notes and tasks
- show a privacy summary of what is currently shared

## Research and evaluation
- test whether users understand the consent flow
- validate that the experience feels trustworthy
- keep prompts gentle and transparent
