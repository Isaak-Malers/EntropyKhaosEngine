# EntropyKhaosEngine
Get in losers, we're learning HA CI/CD IoT Saas.


Goals:

App flow:
1 - ESP32 camera looks at some koi fishes or some other zen imagry.
2 - ESP32 uploads frames to a "Chaos Intake" web service
3 - Chaos Intake service puts frames into a queue
4 - HA scale-able service pulls data from the queue, providing on demand random numbers. 


Ops flow:
1 - all code in one repository
2 - pushing to master branch auto-deploys updates
3 - ESP32 camera auto-updates itself on a regular interval (pulling from github)
4 - Chaos Intake Service is updated on each merge to master (Continuous Delivery)
5 - HA scale-able service is updated on each merge to master (Continuous Deliver)


Environments:
Local environment with docker
Cloud environment based on master branch.