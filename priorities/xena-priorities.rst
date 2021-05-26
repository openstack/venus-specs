.. _xena-themes:

=================
Xena Cycle Themes
=================
PTG:  https://etherpad.opendev.org/p/venus-xena-ptg

Introduction
Venus is the OpenStack project that provides a one-stop solution for
log collection, indexing, analysis, alerting, visualization, report generation
and other needs. Additionally, this project plans to use machine learning
algorithms to quickly locate  failures and root causes, to improve
operation and maintenance efficiency.


TODO
Sign up(deadline March 25th): next PTL's task because "Who will be moderating their discussions?" is one of the question of the survey
https://openinfrafoundation.formstack.com/forms/april2021_vptg_survey
https://ethercalc.net/oz7q0gds9zfi


Background
============

It’s difficult to retrieve logs, since there are many modules in the platform, e.g. systems service, compute, storage, network and other platform services.
Because of  distributed and interaction between components of the cloud platform, and scattered logs between components, it will take more time to locate problems.


Current function
============


Provide a simple and easy-to-use way to retrieve all log and the context .
Realize log association, field value statistics, and provide multi-scene and multi-dimensional visual analysis reports.


Current progress
============

Develop devstack-based depAdd log retrieval of other modules such as vitrage
loyment for venus
Develop the configuration, based on which you can retrieve the chain log of the call


Next step
============

Develop alarm task code to set threshold for the number of error logs of different modules at different times, and provides alarm services and notification services
The configuration, analysis  and alarm of Venus will be integrated into horizon in the form of plugin.
Develop a deployment method based on kolla-ansible
Evaluate whether to collect event data (considering usage, pressure, etc.)
Summarize the log specifications of some typical scenarios and develop them to venus

Promblem
============
Many projects's log records are not standardized, so they can only support full-text retrieval, not multi-dimensional analysis
