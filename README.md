# Confidential Procedure Calls

## Abstract

Confidential virtual machines (CVMs), while providing strong data privacy for cloud tenants, pose significant challenges to VM maintenance like live migration and snapshotting. Traditional host-based maintenance, while applicable to conventional VMs, is infeasible for CVMs due to the lack of trust in the host and the prevention of mandated intrusive access from the host. State-of-the-art approaches depend on non-trivial modifications to hardware and firmware and thus lead to notable compromises in security and/or performance. Furthermore, such approaches lack flexibility for upgrades and cross-platform compatibility, hindering the popularity of CVMs on the cloud.

In this paper, we introduce Confidential Procedure Calls (CPCs), a flexible approach to the efficient and secure execution of CVM maintenance modules from within the guest. We have implemented prototypes on two leading CVM platforms. Our prototype on AMD SEV showcases the high performance of CPCs, with 3× (resource reclamation) or even 138× (live migration) faster than existing approaches. Our prototype on ARM CCA further confirms CPCs' outstanding security and flexibility.

## Conference

This research has been accepted by USENIX ATC'24 and ChinaSys'24.