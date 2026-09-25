# Research architecture and scope

The evaluated path is official paired EMG and measured joint-angle data → frozen pretrained VEMG2Pose prediction → named canonical joint-angle selection → trusted-eight pose representation → independently DB9-trained frozen eight-class LDA consumer. Measured pose follows the same representation and consumer path as a paired reference. No downstream task-specific EMG retraining is evidenced in this chain.

The physical-state boundary requires named degrees of freedom, units, direction, zero, validity, handedness, calibration provenance, and time alignment. Name matching alone does not establish numerical equivalence across sources. Cross-source physical zero and calibration equality remain unresolved.

For each eligible 50-Hz block, Flip is one when the consumer class under predicted pose differs from its class under measured pose. A reliability gate ranks blocks using information available at serving time. The reported selective evaluation retains the lowest-score 30% **within each user** and abstains on the others. This evaluation rule is not evidence that one global deployment threshold would yield 30% coverage for every future user.

Gate4E targets ordinary usage-weighted Flip risk. Gate4F targets class-balanced Flip risk, averaging supported measured-pose reference classes; its frozen support rule requires at least 30 accepted blocks for a class to contribute. Gate4D studied a separate continuous seven-dimensional Fisher-space error on development users. These objectives must be interpreted separately.

This is an offline, consumer-specific research path. It does not establish a universal Human State API, semantic gesture recognition, online latency, or clinical or product safety.
