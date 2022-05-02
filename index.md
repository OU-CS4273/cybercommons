---
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
marp: true
backgroundImage: url('https://marp.app/assets/hero-background.svg')
---

![bg left:50% 100%](https://libraries.ou.edu/sites/all/themes/oulib_bootstrap/img/ou_lib_logo.png)

# **OU Library Testing with Cybercommons**

Group 1 - Kenton Huff, Julie Nguyen, Jennifer Pham, Grace Wu


---

# What is Cybercommons?

</br>

* OU IT Library framework that manages data, catalog metadata, and contains defined tasks
* uses a Python API along with Docker
* Also uses MongoDB, RabbitMQ, Django, and Celery
* workspace of our project

---
# GitPod

![bg left:40% 70%](https://avatars.githubusercontent.com/u/37021919?s=200&v=4)

</br>

* Access to online IDE
* connects github repo to bypass environment dependencies
* Environment already set up

---
# Test We Wrote

```python

def test_islandora_ingest_recipe(self):
        request = self.factory.post('/queue/run/islandoraq.tasks.tasks.
        ingest_recipe/', {"function": "islandoraq.tasks.tasks.ingest_recipe",
        "queue": "repository-islandora-test-workerq","args": ["https://bag.ou.
        edu/derivative/Darwin_1864/jpeg_040_antialias/darwin_1864.json"],
        "kwargs": {},"tags": []}, format='json')
        force_authenticate(request, user=self.user)
        response = self.userprofile_view(request)
        self.assertEqual(response.status_code,status.HTTP_200_OK)

```
---
# Demonstration

</br>

* insert link

---
# Why it's important

</br>

* something


--- 
# Hurdles/Obstacles

</br>

* Getting the Environment set up
* Making sure the tasks are running correctly


---

# **Questions?**

