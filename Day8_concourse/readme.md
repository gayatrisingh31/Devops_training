### Question/Answer

### Ques. What is the difference between Build and Task?

Ans. The smallest configurable unit in a Concourse pipeline is a single task. A task can be thought of as a function from a task. inputs to tasks. outputs that can either succeed or fail. Each job has a build plan declaring the job's input resources and what to run with them when they change.

### Ques. Difference between resource and Resource type?

Ans. A resource type is an image and we need to configure the repository and tag in its source so that the concourse can locate/download it. A resource is a container which is an instance of that image and can be used in the jobs when the pipeline is running. Its source that we configure is the common parameters which will be passed on the stdin to the check, in and out scripts when the resource is configured in a get or put step.

### Ques. What is a webnode?

Ans. The web node is responsible for running the web UI, API, and as well as performing all pipeline scheduling. It's basically the brain of Concourse.

### Ques. What is a worker node?

Ans. The worker node registers with the web node and is then used for executing builds and performing resource checks.

### Ques. How do ATC & TSA communicate?

Ans. The ATC is the heart of Concourse. It runs the web UI and API and is responsible for all pipeline scheduling. It connects to PostgreSQL, which it uses to store pipeline data (including build logs). The TSA is a custom-built SSH server that is used solely for securely registering workers with the ATC. The TSA by default listens on port 2222, and is usually co-located with the ATC and sitting behind a load balancer.

### Ques. Where does the worker node run in our system?

Ans. The worker node registers with the web node and is then used for executing builds and performing resource checks. It doesn't really decide much on its own. CONCOURSE_WORK_DIR=/opt/concourse/worker

### Ques. Study full workflow and architecture of Concourse

Ans. Concourse software components can be logically split into two main subsystems: a web (or server) subsystem, and one or more workers. In a less complicated setup, both subsystems can run on a single VM. In more complex systems, Concourse web and worker subsystems run on multiple VMs. This diagram shows a Concourse deployment with web and server subsystems on separate VMs. You can deploy each subsystem on a single VM, as shown, or on multiple VMs in parallel. A dedicated database VM runs Concourse’s PostgreSQL server. If needed, an optional load balancer points external traffic to web VMs.

### Ques. Difference between error and failed

Ans. A mistake in coding is called Error, error found by tester is called Defect, defect accepted by development team then it is called Bug, build does not meet the requirements then it Is Failure. Error : Refers to difference between Actual Output and Expected output. Failure : It is the inability of a system or component to perform required function according to its specification.

### Ques. How many ways are there to run a task?

Ans. As soon as your local concourse instance is online, run task_hello_world.yml directly from the command line with the following fly command: fly -t tutorial execute -c task_hello_world.yml


