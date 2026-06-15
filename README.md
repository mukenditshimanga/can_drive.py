# Function 
def can_drive(age):
    driving_age = 16
    return age >= driving_age


class TestCanDrive(unittest.TestCase):

    def test_underage(self):
        self.assertFalse(can_drive(15))

    def test_exact_age(self):
        self.assertTrue(can_drive(16))

    def test_over_age(self):
        self.assertTrue(can_drive(18))

    def test_zero_age(self):
        self.assertFalse(can_drive(0))

    def test_negative_age(self):
        self.assertFalse(can_drive(-5))


if __name__ == "__main__":
    unittest.main()
