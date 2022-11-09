# Reliability

#Programming #DDI #Software\ Architecture

> Software that works correctly, even when things go wrong

## Handling faults

> fault - one component of a system not working
> failure - all the system not working

### Hardware

- **redundancy**: backup power, RAID configuration of disks, hot-swappable [[37ve-processors|cpus]]; does not prevent faults, but keeps the machine running
- **software fault-tolerance**: multi-core servers ???

### Software

- bugs, multiple faults, low efficiency etc.

### Human errors

- leading cause of faults
- design systems that make it "easy to do the right thing" and "hard to do the wrong thing"
- create sandboxes for teaching and experimenting safely
- through testing
- telemetry is essential for tracking what is happening in big applications
