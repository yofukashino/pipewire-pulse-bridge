# pipewire-pulse-bridge

Bridge that allows applications which only support PulseAudio (such as Discord) to capture audio streams from a PipeWire.

## Why this exists

Because fuck me. Nah mate for fucking real, discord will use pipewire for capturing video stream but audio nah. "Pulse Audio is best we can do"

I waited a while to write this hoping discord will fix their shit but instead they focus on age verification. So wrote this to kill bordem while discord dies.

## Info

- `pipewire-pulse-bridge`
  - This is just a wrapper to make it easy
  - Every command can be ran outside of wrapper but would require multiple shells to end cleanly
- `venmic-server`
  - This is the rust binary built from [Vencord/venmic](https://github.com/Vencord/venmic) (For those who don't wanna build themselves)
  - Runs on port `30212` by default, can be edited in wrapper
  - Captures every app which is non running via pulse audio can be edited in wrapper


## Usage
- Clone the repo, and cd in  (`git clone https://github.com/yofukashino/pipewire-pulse-bridge & cd pipewire-pulse-bridge`)
- Mark script/binary as executeable (`chmod +x ./pipewire-pulse-bridge & chmod +x ./venmic-server`)
- Run `pipewire-pulse-bridge` (`pipewire-pulse-bridge`)

Doesn't matter if you run this before or after starting discord stream. 

## Install

Not planned, PR's are welcome. Basically just fetch the script and wrapper and link to `~/.local/bin` maybe. 


# Thanks to [Vencord/venmic](https://github.com/Vencord/venmic) for `venmic-server`.

btw if `venmic-server` binary is published somewhere officially let me know. 
