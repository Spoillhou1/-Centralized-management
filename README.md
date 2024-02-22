class CentralizedManagement:
    def __init__(self):
        self.resources = []

    def add_resource(self, resource):
        self.resources.append(resource)

    def remove_resource(self, resource):
        self.resources.remove(resource)

    def display_resources(self):
        print("Resources managed:")
        for resource in self.resources:
            print(resource)

# Example usage
manager = CentralizedManagement()
manager.add_resource("Resource 1")
manager.add_resource("Resource 2")
manager.add_resource("Resource 3")

manager.display_resources()

manager.remove_resource("Resource 2")

manager.display_resources()
