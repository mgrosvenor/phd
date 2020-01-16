# Latency-First Datacenter Network Scheduling 

**Overview**

This repository is a public store for the final result of my PhD dissertation on latency control in datacenter networks. There are two versions:

- [thesis.pdf](https://github.com/mgrosvenor/phd/blob/master/thesis.pdf) which is a short version of the document, intended for faster downloads and easier digital viewing.  
- [thesis-full.pdf]() which is a fully prinable final version. This version includes a full copy of Appendix A, which includes extracts of web-based resources used inthe document, but which may expire or be removed by their auhtors. This is considered fair-use from a copyright perspecitve. 

**Citing**

This disseration is also published as [Technical Report number 943](https://www.cl.cam.ac.uk/techreports/UCAM-CL-TR-943.html) by the University of Cambridge Computer Laboratory. You can cite the technical report using the following BibTeX record. 

```
@TechReport{UCAM-CL-TR-943,
  author =	 {Grosvenor, Mathew P.},
  title = 	 {{Latency-First datacenter network scheduling}},
  year = 	 2020,
  month = 	 jan,
  url = 	 {https://www.cl.cam.ac.uk/techreports/UCAM-CL-TR-943.pdf},
  institution =  {University of Cambridge, Computer Laboratory},
  number = 	 {UCAM-CL-TR-943}
}
```

**Summary**

Every day we take for granted that, with the click of a mouse or a tap on a touchscreen, we can instantly access the Internet to globally exchange information, finances and physical goods. The computational machinery behind the Internet is found in datacenters scattered all over the globe. Each datacenter contains many tens of thousands of computers connected together through a datacenter network. Like the Internet, datacenter networks suffer from network interference. Network interference occurs when congestion caused by some applications, delays or interferes with traffic from other applications. Network interference makes it difficult to predict network latency: the time that any given packet will take to traverse the network. The lack of predictability makes it difficult to build fast, efficient, and responsive datacenter applications.

In this dissertation I address the problem of network interference in datacenter networks. I do so primarily by exploiting network scheduling techniques. Network scheduling techniques were previously developed to provide predictability in the Internet. However, they were complex to deploy and administer because few assumptions could be made about the network. Unlike the Internet, datacenter networks are administered by a single entity, and have well known physical properties, that rarely change.

The thesis of this dissertation is that it is both possible and practical to resolve network interference in datacenter networks by using network scheduling techniques. I show that it is possible to resolve network interference by deriving a simple, and general, network scheduler and traffic regulator. I take the novel step of basing my scheduler design on a simple, but realistic, model of a datacenter switch. By regulating the flow of traffic into each switch, I show that it is possible to bound latency across the network. I develop the leaky token bucket regulator to perform this function. 

I show that my network scheduler design is practical by implementing a simple, and immediately deployable, system called QJUMP. QJUMP is thoroughly evaluated and demonstrated to resolve network interference between datacenter applications in both simulation and on a physical test-bed. I further show that QJUMP can be extended and improved upon in a variety of ways. I therefore conclude that it is both possible and practical to control network interference in datacenter networks using network scheduling techniques.

