# Function 
def can_drive(age):
    driving_age = 16
    return age >= driving_age


class TestCanDrive(unittest.TestCase):

    def test_driving.eligibility(self):
       #Test Eligibility
       self.assertTrue(can_drive(25))
       self.assertTrue(can_drive(17))
       self.assertTrue(can_drive(16))

       #Test Ineligibible
       sel.assertFalse(can_drive(15))
       self.assertFalse(can_drive(0))
       self.assertFalse(can_drive(-1)


if __name__ == "__main__":
    unittest.main()
