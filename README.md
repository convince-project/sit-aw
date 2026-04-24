# sit-aw

sit-aw is a software pipeline for robot situation awareness, part of the [CONVINCE toolchain](https://convince-project.github.io/overview/). It enables known and unknown anomaly detection, identification and resolution.

Below there is a list of the available software modules in the different releases of the sit-aw pipeline. Each module is provided with documentation that contains a tutorial demonstrating the module functionality.

## 0.2.0 (End of October 2025)

- [sit-aw-anchoring](https://github.com/convince-project/sit-aw-anchoring), the semantic anchoring module.

   Semantic anchoring is the process in the robot situation awareness pipeline that integrates numerical data coming from perception with information in one (or more) digital twin(s), to produce a symbolic representation (belief) of current and predicted observations of operational environment.

- [sit-aw-aip](https://github.com/convince-project/sit-aw-aip), Vision-Language Model (VLM)-based pipeline for the identification of situational anomalies in robot operation.

  Anomalies correspond to failures that may occur and interrupt the nominal behaviour of the robot while performing its computed task. Our Anomaly Identification Pipeline (AIP) considers failures that designers thought about and compiled within a list, along with an "unknown" class that represents all the others.

- [sit-aw-critics](https://github.com/convince-project/sit-aw-critics), logic rules (critics) and inference to detect and reduce hallucinations of general-purpose AI like multi-modal large language models.

  Critics principle is to use expert algorithms to detect the hallucinations in the VLM response, and then do a new call to the VLM API with an updated prompt to correct the previously detected hallucination.
